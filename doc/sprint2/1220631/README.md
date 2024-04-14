# RCOMP 2023-2024 Project - Sprint 2 - Member 1220631 Folder

## VLAN database and IPv4 network

### Building 2 IPv4 Network Table

| Network                   | IP Address    | Subnet Mask Prefix |
|---------------------------|---------------|--------------------|
| Ground Floor (90 Nodes)   | 172.25.36.0   | /25                |
| 1st Floor (120 Nodes)     | 172.25.36.128 | /25                |
| Wi-fi Network (220 Nodes) | 172.25.37.0   | /24                |
| DMZ (50 Nodes)            | 172.25.38.128 | /26                |
| VOIP (110 Nodes)          | 172.25.38.0   | /25                |


### Building 2 VLAN-IPv4 network database/table

| Network       | VLAN ID | VLAN Name         | Total of Nodes | IP Address       | First Host    | Last Host     | Broadcast     | Sub-netting mask |
|---------------|---------|-------------------|----------------|------------------|---------------|---------------|---------------|------------------|
| Ground Floor  | 411     | GFBuilding2       | 90             | 172.25.36.0/25   | 172.25.36.1   | 172.25.36.126 | 172.25.36.127 | 255.255.255.128  |
| 1st Floor     | 412     | FFBuilding2       | 120            | 172.25.36.128/25 | 172.25.36.129 | 172.25.36.254 | 172.25.36.255 | 255.255.255.128  |
| Wi-fi Network | 413     | WirelessBuilding2 | 220            | 172.25.37.0/24   | 172.25.37.1   | 172.25.37.254 | 172.25.37.255 | 255.255.255.0    |
| DMZ           | 414     | DMZBuilding2      | 50             | 172.25.38.128/26 | 172.25.38.129 | 172.25.38.190 | 172.25.38.191 | 255.255.255.192  |
| VOIP          | 415     | VOIPBuilding2     | 110            | 172.25.38.0/25   | 172.25.38.1   | 172.25.38.126 | 172.25.38.127 | 255.255.255.128  |

### Building 2

[Project (open with Cisco Packet Tracer)][building_2.pkt](..%2F..%2F..%2F..%2F..%2FDownloads%2Fsprint2%2Fsprint2%2F1201205%2Fbuilding_2.pkt)

#### Image

![building_2.PNG](images%2Fbuilding_2.PNG)


#### Config Files

| Switch/Router | Config File                                          |
|---------------|------------------------------------------------------|
| CP2-003       | [Config](config-files%2FSwitch_CP_B2_F0_1_startup-config.txt) |
| CP2-102       | [Config](config-files%2FSwitch_CP_B2_F1_1_startup-config.txt) |
| HCC2-011      | [Config](config-files%2FSwitch_HC_B2_F0_startup-config.txt) |
| HCC2-112      | [Config](config-files%2FSwitch_HC_B2_F1_startup-config.txt) |
| ICC2-011      | [Config](config-files%2FSwitch_IC_B2_startup-config.txt) |
| RT2           | [Config](config-files%2FRouter_B2_startup-config.txt) |
