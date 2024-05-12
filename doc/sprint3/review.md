# RCOMP 2023-2024 Project

- #### Class: 2DJ
- #### Group: 4

# Sprint 3 Review

## Sprint 3 Backlog

| Task  | Completion state              |
|-------|-------------------------------|
| T.3.1 | Everything done besides acl's |
| T.3.2 | Everything done besides acl's |
| T.3.3 | Not completed                 |
| T.3.4 | Everything done               |


## DHCP Configuration

Dhcp service was configured in all buildings, with the following configurations:


| Network               | IP Address  | Subnet Mask Prefix |
|-----------------------|-------------|--------------------|
| Backbone & Building 1 | 172.25.32.0 | /22                |
| Building 2            | 172.25.36.0 | /22                |
| Building 3            | 172.25.40.0 | /22                |
| Building 4            | 172.25.44.0 | /22                |


### Building 1

| Network                  | IP Address    | Subnet Mask Prefix |
|--------------------------|---------------|--------------------|
| Ground Floor (50 Nodes)  | 172.25.33.0   | /26                |
| 1st Floor (50 Nodes)     | 172.25.33.64  | /26                |
| Wi-fi Network (80 Nodes) | 172.25.33.128 | /25                |
| VOIP (67 Nodes)          | 172.25.34.128 | /25                |

### Building 2

| Network                   | IP Address    | Subnet Mask Prefix |
|---------------------------|---------------|--------------------|
| Ground Floor (90 Nodes)   | 172.25.36.0   | /25                |
| 1st Floor (120 Nodes)     | 172.25.36.128 | /25                |
| Wi-fi Network (220 Nodes) | 172.25.37.0   | /24                |
| VOIP (110 Nodes)          | 172.25.38.0   | /25                |


### Building 4

| Network                   | IP Address    | Subnet Mask Prefix |
|---------------------------|---------------|--------------------|
| Ground Floor (120 Nodes)  | 172.25.44.0   | /25                |
| 1st Floor (150 Nodes)     | 172.25.45.0   | /24                |
| Wi-fi Network (190 Nodes) | 172.25.46.0   | /24                |
| VOIP (170 Nodes)          | 172.25.47.0   | /24                |


## OSPF Configuration

The OSPF routing protocol was configured in all buildings, with the following configurations:

- **OSPF Area 0** was used as the backbone area.
- **OSPF Area N** was used as the area for each building, where `N` is the building number.
- The OSPF process ID was **100**.
- The router id was **N.N.N.N**, where `N` is the building number.

## VOIP Service Configuration

The VOIP numbering plan was configured as follows:

- The IP Phones number should look like **NXXX**, where `N` is the building number and `XXX` is the phone number.

## DNS Configuration

The DNS servers were configured as follows:

- The server previously placed in the DMZ was configured as a DNS server.
- The name of the servers was ns.rcomp-23-24-2dj-g4 in **Building 1**, and ns.buildingN.rcomp-23-24-2dj-g4 in the other buildings.
- The root domain name was **rcomp-23-24-2dj-g4**, and this acted as the domain name for **Building 1**.
- The other buildings had a local subdomain named as follows: `buildingN.rcomp-23-24-2dj-g4`, where `N` was the building number.
- All DNS servers had the unqualified DNS name ns, so for building 1 it was ns.rcomp-23-24-cc-gn, and for instance for building 3 it was ns.building-3.rcomp-23-24-cc-gn.
- All HTTP servers were named as server1 (A record).
- Within each DNS domain there was a www alias (CNAME) mapped to the same domain’s server1 A record, and another alias, named web also mapped to the domain’s server1 A record.
- One additional alias (CNAME), with name dns, and mapped to the domain’s ns A record, existed.
- The DNS servers IP Addressing was as follows:

![DNS-Database.png](1220631%2FDNS-Database.png)
![DNS-Database.png](1221083%2FDNS-Database.png)
![DNS-Database.png](1221276%2FDNS-Database.png)

## Web Server

The web server was configured as follows:

- All HTTP servers were named as server1 (A record).
- Within each DNS domain there was a www alias (CNAME) mapped to the same domain’s server1 A record, and another alias, named web also mapped to the domain’s server1 A record.
- One additional alias (CNAME), with name dns, and mapped to the domain’s ns A record, existed.

## ACL's

Most acl's are no functional.

This is the configuration of the acl's that are functional:

### WIRELESS BUILDING 4

- block the traffic to the router interfaces:
```bash
access-list 103 deny ip any host 172.25.44.126 
access-list 103 deny ip any host 172.25.45.254
access-list 103 deny ip any host 172.25.46.254
access-list 103 deny ip any host 172.25.44.190
access-list 103 deny ip any host 172.25.47.254
```

-only allow icmp, http, https and dns traffic to the servers:
```bash
access-list 103 permit icmp any 172.25.44.128 0.0.0.63 echo-reply
access-list 103 permit tcp any 172.25.44.128 0.0.0.63 eq www
access-list 103 permit tcp any 172.25.44.128 0.0.0.63 eq 443
access-list 103 permit udp any 172.25.44.128 0.0.0.63 eq domain
```

-allow the traffic to the other networks:
```bash
access-list 103 deny ip any 172.25.44.128 0.0.0.63
access-list 103 permit ip 172.25.46.0 0.0.0.255 any
access-list 103 permit udp any eq bootpc any eq bootps
```

### ANTI SPOOFING BUILDING 4
    
- allow tcp and udp traffic in the backbone network:
```bash
access-list 100 deny ip 172.25.44.128 0.0.0.63 any
access-list 100 permit tcp any 172.25.44.128 0.0.0.63 eq 80
access-list 100 permit tcp any 172.25.44.128 0.0.0.63 eq 443
access-list 100 permit udp any 172.25.44.128 0.0.0.63 eq 53
access-list 100 permit udp any eq 53 172.25.44.128 0.0.0.63
```

- allow traffic from the other networks:
```bash
access-list 100 deny ip 172.25.44.0 0.0.0.127 any
access-list 100 deny ip any host 172.25.44.126
access-list 100 permit ip any 172.25.44.0 0.0.0.127



access-list 100 deny ip 172.25.45 0.0.0.255 any
access-list 100 deny ip any host 172.25.45.254
access-list 100 permit ip any 172.25.45 0.0.0.255

access-list 100 deny ip 172.25.46.0 0.0.0.255 any
access-list 100 deny ip any host 172.25.46.254
access-list 100 permit ip any 172.25.46.0 0.0.0.255

access-list 100 deny ip 172.25.47 0.0.0.255 any
access-list 100 permit ip any host 172.25.47.254
access-list 100 permit ip any 172.25.47 0.0.0.255

access-list 100 deny ip any host 172.25.44.190
```

- allow dhcp and ospf traffic
```bash
access-list 100 permit icmp any 172.25.44.128 0.0.0.63 echo-reply
access-list 100 permit ospf any any
```

### VOIP BUILDING 4

- block the traffic to the router interfaces:
```bash
access-list 105 deny ip any host 172.25.44.126
access-list 105 deny ip any host 172.25.45.254
access-list 105 deny ip any host 172.25.46.254
access-list 105 deny ip any host 172.25.44.190
```

- allow icmp, http, https and dns traffic to the servers and block other communication to the servers:
```bash
access-list 105 permit icmp any 172.25.44.128 0.0.0.63 echo-reply
access-list 105 permit tcp any 172.25.44.128 0.0.0.63 eq www
access-list 105 permit tcp any 172.25.44.128 0.0.0.63 eq 443
access-list 105 permit udp any 172.25.44.128 0.0.0.63 eq domain
access-list 105 deny ip any 172.25.44.128 0.0.0.63
access-list 105 permit ip 172.25.47.0 0.0.0.255 any
access-list 105 permit udp any eq bootpc any eq bootps
```

### First Floor BUILDING 4

- block the traffic to the router interfaces:
```bash
access-list 102 deny ip any host 172.25.44.126
access-list 102 deny ip any host 172.25.45.254
access-list 102 deny ip any host 172.25.46.254
access-list 102 deny ip any host 172.25.47.254
access-list 102 deny ip any host 172.25.44.254
```

- allow icmp, http, https and dns traffic to the servers and block other communication to the servers:
```bash
access-list 102 permit icmp any 172.25.44.128 0.0.0.63 echo-reply
access-list 102 permit tcp any 172.25.44.128 0.0.0.63 eq www
access-list 102 permit tcp any 172.25.44.128 0.0.0.63 eq 443
access-list 102 permit udp any 172.25.44.128 0.0.0.63 eq domain
access-list 102 deny ip any 172.25.44.128 0.0.0.63
access-list 102 permit ip 172.25.45.0 0.0.0.255 any
access-list 102 permit udp any eq bootpc any eq bootps
```

### Ground Floor BUILDING 4

- block the traffic to the router interfaces:
```bash
access-list 101 deny ip any host 172.25.44.126
access-list 101 deny ip any host 172.25.45.254
access-list 101 deny ip any host 172.25.46.254
access-list 101 deny ip any host 172.25.44.190
access-list 101 deny ip any host 172.25.47.254
```

- allow icmp, http, https and dns traffic to the servers and block other communication to the servers:
```bash
access-list 101 permit icmp any 172.25.44.128 0.0.0.63 echo-reply
access-list 101 permit tcp any 172.25.44.128 0.0.0.63 eq www
access-list 101 permit tcp any 172.25.44.128 0.0.0.63 eq 443
access-list 101 permit udp any 172.25.44.128 0.0.0.63 eq domain
access-list 101 deny ip any 172.25.44.128 0.0.0.63
access-list 101 permit ip 172.25.44.0 0.0.0.127 any
access-list 101 permit udp any eq bootpc any eq bootps
```




