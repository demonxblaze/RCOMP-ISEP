# RCOMP 2023-2024 Project - Sprint 2 - Member 1221083 Folder

## VLAN database and IPv4 network

### Building 1 IPv4 network diagram

![](images/Building_1_IPV4.svg)

### Campus Backbone IPv4 network diagram

![](images/Backbone_IPV4.svg)

### Building 1 VLAN-IPv4 network database/table

| Network       | VLAN ID | VLAN Name             | Total of Nodes | IP Address       | First Host    | Last Host     | Broadcast     | Sub-netting mask |
|---------------|---------|-----------------------|----------------|------------------|---------------|---------------|---------------|------------------|
| Ground Floor  | 406     | GFBuilding1VLAN       | 50             | 172.25.33.0/26   | 172.25.33.1   | 172.25.33.62  | 172.25.33.63  | 255.255.255.192  |
| 1st Floor     | 407     | FFBuilding1VLAN       | 50             | 172.25.33.64/26  | 172.25.33.65  | 172.25.33.126 | 172.25.33.127 | 255.255.255.192  |
| Wi-fi Network | 408     | WirelessBuilding1VLAN | 80             | 172.25.33.128/25 | 172.25.33.129 | 172.25.33.254 | 172.25.33.255 | 255.255.255.128  |
| DMZ           | 409     | DMZBuilding1VLAN      | 100            | 172.25.34.0/25   | 172.25.34.1   | 172.25.34.126 | 172.25.34.127 | 255.255.255.128  |
| VOIP          | 410     | VOIPBuilding1VLAN     | 67             | 172.25.34.128/25 | 172.25.34.129 | 172.25.35.254 | 172.25.35.255 | 255.255.255.128  |

### Building 1

[Project (open with Cisco Packet Tracer)](building1.pkt)

#### Image

![](images/Building_1.png)

#### Pings

**DMZ1-17**

![](images/pings/DMZ1-17.png)

**LP1-01** 

![](images/pings/LP1-01.png)
**LP1-16** 

![](images/pings/LP1-16.png)
**PC1-02** 

![](images/pings/PC1-02.png)
**PC1-06** 

![](images/pings/PC1-06.png)
**PC1-12** 

![](images/pings/PC1-12.png)
**PC1-14** 

![](images/pings/PC1-14.png)

#### Config Files

| Switch/Router | Config File                                            |
|---------------|--------------------------------------------------------|
| CP1-02        | [Config File](config-files/CP1-02_startup-config.txt)  |
| CP1-05        | [Config File](config-files/CP1-05_startup-config.txt)  |
| CP1-13        | [Config File](config-files/CP1-13_startup-config.txt)  |
| CP1-15        | [Config File](config-files/CP1-15_startup-config.txt)  |
| HCC1-04       | [Config File](config-files/HCC1-04_startup-config.txt) |
| HCC1-14       | [Config File](config-files/HCC1-14_startup-config.txt) |
| ICC1-14       | [Config File](config-files/ICC1-14_startup-config.txt) |
| MCC1-14       | [Config File](config-files/MCC1-14_startup-config.txt) |
| RT1-14        | [Config File](config-files/RT1-14_startup-config.txt)  |
| RT1-X         | [Config File](config-files/RT1-X_startup-config.txt)   |
| RT_ISP        | [Config File](config-files/RT_ISP_startup-config.txt)  |

### Campus

[Project (open with the Cisco Packet Tracer)](campus.pkt)
