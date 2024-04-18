# RCOMP 2023-2024 Project - Sprint 2 - Member 1221276 Folder

## VLAN database and IPv4 network

### Building 4 IPv4 Network Table

| Network                   | IP Address    | Subnet Mask Prefix |
|---------------------------|---------------|--------------------|
| Ground Floor (120 Nodes)  | 172.25.44.0   | /25                |
| 1st Floor (150 Nodes)     | 172.25.45.0   | /24                |
| Wi-fi Network (190 Nodes) | 172.25.46.0   | /24                |
| DMZ (40 Nodes)            | 172.25.44.128 | /26                |
| VOIP (170 Nodes)          | 172.25.47.0   | /24                |


### Building 1 VLAN-IPv4 network database/table

| Network       | VLAN ID | VLAN Name         | Total of Nodes | IP Address       | First Host    | Last Host     | Broadcast     | Sub-netting mask |
|---------------|---------|-------------------|----------------|------------------|---------------|---------------|---------------|------------------|
| Ground Floor  | 421     | GFBuilding4       | 120            | 172.25.44.0/25   | 172.25.44.1   | 172.25.44.126 | 172.25.44.127 | 255.255.255.128  |
| 1st Floor     | 422     | FFBuilding4       | 150            | 172.25.45.0/24   | 172.25.45.1   | 172.25.45.254 | 172.25.45.255 | 255.255.255.0    |
| Wi-fi Network | 423     | WirelessBuilding4 | 190            | 172.25.46.0/24   | 172.25.46.1   | 172.25.46.254 | 172.25.46.255 | 255.255.255.0    |
| DMZ           | 424     | DMZBuilding4      | 40             | 172.25.44.128/26 | 172.25.44.129 | 172.25.44.190 | 172.25.44.191 | 255.255.255.192  |
| VOIP          | 425     | VOIPBuilding4     | 170            | 172.25.47.0/24   | 172.25.47.1   | 172.25.47.254 | 172.25.35.255 | 255.255.255.0    |

### Building 1

[Project (open with Cisco Packet Tracer)](building4.pkt)

#### Image

![building4.PNG](images%2Fbuilding4.PNG)

#### Pings

**GF CONNECTIVITY**

![CONECTIVITY_GF4.PNG](images%2FCONECTIVITY_GF4.PNG)

**FF CONNECTIVITY**

![CONECTIVITY_FF4.PNG](images%2FCONECTIVITY_FF4.PNG)

**WIRELESS CONNECTIVITY**

![CONECTIVITY_WIRELESS4.PNG](images%2FCONECTIVITY_WIRELESS4.PNG)

**DMZ CONNECTIVITY**

![CONECTIVITY_DMZ4.PNG](images%2FCONECTIVITY_DMZ4.PNG)


#### Config Files

| Switch/Router | Config File                                          |
|---------------|------------------------------------------------------|
| CP4-003       | [Config](config-files%2FCP4-003_startup-config.txt)  |
| CP4-101       | [Config](config-files%2FCP4-101_startup-config.txt)  |
| HCC4-012      | [Config](config-files%2FHCC4-012_startup-config.txt) |
| HCC4-119      | [Config](config-files%2FHCC4-119_startup-config.txt) |
| ICC4-012      | [Config](config-files%2FICC4-012_startup-config.txt) |
| RT4           | [Config](config-files%2FRT4_startup-config.txt)      |


