# RCOMP 2023-2024 Project

- #### Class: 2DJ
- #### Group: 4

# Sprint 2 Planning

## Sprint 2 Backlog
| Task   | Task description                                                                                                                                                                                       |
|--------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| T.2.1  | Development of a layer two and layer three Packet Tracer simulation for building 1, encompassing the campus backbone. Integration of every member’s Packet Tracer simulation into a single simulation. |
| T.2.2  | Development of a layer two and layer three Packet Tracer simulation for building 2, encompassing the campus backbone.                                                                                  |
| T.2.3  | Development of a layer two and layer three Packet Tracer simulation for building 3, encompassing the campus backbone.                                                                                  |
| T.2.4  | Development of a layer two and layer three Packet Tracer simulation for building 4, encompassing the campus backbone.                                                                                  |

## Sprint 2 Task Assignments

**T.2.1** - **1221083**

**T.2.2** - **1220631**

**T.2.4** - **1221276**

## Packet Tracer Simulation

The Packet Tracer simulation will be developed using the following guidelines:
- Version: Packet Tracer 8.2.1.118
- Every building will have a separate Packet Tracer file, that should be named as follows: `buildingN.pkt`, where `N` is the building number.
- All configuration files should be exported as a `.txt` file and stored in the repository.

## Device Naming Convention

The devices display names and hostnames should be named according to the following convention:
XXXN-FRR, where:
- `XXX` is the device type (`CP` for Consolidation Points, `HCC` for Horizontal Cross Connects, `ICC` for Intermediate Cross Connect,`RT` for routers, etc...)
- `N` is the building number
- `F` is the floor number
- `R` is the room number

## VLAN Distribution And VTP Domain

**Available VLANs:** 406 – 427

**VTP Domain Name:** `r2324djg4`

### VLAN Distribution

#### Campus Backbone

| Network  | VLAN ID | VLAN Name     |
|----------|---------|---------------|
| Backbone | 427     | Backbone VLAN |

#### Building 1

| Network       | VLAN ID | VLAN Name                |
|---------------|---------|--------------------------|
| Ground Floor  | 406     | GF Building 1 VLAN       |
| 1st Floor     | 407     | FF Building 1 VLAN       |
| Wi-fi Network | 408     | Wireless Building 1 VLAN |
| DMZ           | 409     | DMZ Building 1 VLAN      |
| VOIP          | 410     | VOIP Building 1 VLAN     |

#### Building 2

| Network       | VLAN ID | VLAN Name                |
|---------------|---------|--------------------------|
| Ground Floor  | 411     | GF Building 2 VLAN       |
| 1st Floor     | 412     | FF Building 2 VLAN       |
| Wi-fi Network | 413     | Wireless Building 2 VLAN |
| DMZ           | 414     | DMZ Building 2 VLAN      |
| VOIP          | 415     | VOIP Building 2 VLAN     |
    
#### Building 3

| Network       | VLAN ID | VLAN Name                |
|---------------|---------|--------------------------|
| Ground Floor  | 416     | GF Building 3 VLAN       |
| 1st Floor     | 417     | FF Building 3 VLAN       |
| Wi-fi Network | 418     | Wireless Building 3 VLAN |
| DMZ           | 419     | DMZ Building 3 VLAN      |
| VOIP          | 420     | VOIP Building 3 VLAN     |

#### Building 4

| Network               | VLAN ID | VLAN Name                |
|-----------------------|---------|--------------------------|
| Ground Floor          | 421     | GF Building 4 VLAN       |
| 1st Floor             | 422     | FF Building 4 VLAN       |
| Wi-fi Network         | 423     | Wireless Building 4 VLAN |
| DMZ                   | 424     | DMZ Building 4 VLAN      |
| VOIP                  | 425     | VOIP Building 4 VLAN     |


## Building IP Addressing

**Base IP Address:** `172.25.32.0 /20`

| Network               | IP Address  | Subnet Mask Prefix |
|-----------------------|-------------|--------------------|
| Backbone & Building 1 | 172.25.32.0 | /22                |
| Building 2            | 172.25.36.0 | /22                |
| Building 3            | 172.25.40.0 | /22                |
| Building 4            | 172.25.44.0 | /22                |

## Subnetting

### Building 1

| Network                  | IP Address    | Subnet Mask Prefix |
|--------------------------|---------------|--------------------|
| Ground Floor (50 Nodes)  | 172.25.33.0   | /26                |
| 1st Floor (50 Nodes)     | 172.25.33.64  | /26                |
| Wi-fi Network (80 Nodes) | 172.25.33.128 | /25                |
| DMZ (100 Nodes)          | 172.25.34.0   | /25                |
| VOIP (67 Nodes)          | 172.25.34.128 | /25                |
| Backbone (200 Nodes)     | 172.25.32.0   | /24                |

### Building 2

| Network                   | IP Address    | Subnet Mask Prefix |
|---------------------------|---------------|--------------------|
| Ground Floor (90 Nodes)   | 172.25.36.0   | /25                |
| 1st Floor (120 Nodes)     | 172.25.36.128 | /25                |
| Wi-fi Network (220 Nodes) | 172.25.37.0   | /24                |
| DMZ (50 Nodes)            | 172.25.38.0   | /26                |
| VOIP (110 Nodes)          | 172.25.38.64  | /25                |

### Building 3

| Network                   | IP Address    | Subnet Mask Prefix |
|---------------------------|---------------|--------------------|
| Ground Floor (110 Nodes)  | 172.25.40.0   | /25                |
| 1st Floor (130 Nodes)     | 172.25.41.0   | /24                |
| Wi-fi Network (200 Nodes) | 172.25.42.0   | /24                |
| DMZ (45 Nodes)            | 172.41.40.128 | /26                |
| VOIP (180 Nodes)          | 172.25.43.0   | /24                |

### Building 4

| Network                   | IP Address    | Subnet Mask Prefix |
|---------------------------|---------------|--------------------|
| Ground Floor (120 Nodes)  | 172.25.44.0   | /25                |
| 1st Floor (150 Nodes)     | 172.25.45.0   | /24                |
| Wi-fi Network (190 Nodes) | 172.25.46.0   | /24                |
| DMZ (40 Nodes)            | 172.25.44.128 | /26                |
| VOIP (170 Nodes)          | 172.25.47.0   | /24                |

### Routers

|Building | IP Address  | Subnet Mask Prefix |
|---------|-------------|--------------------|
|1        | 172.25.32.1 | /24                |
|2        | 172.25.32.2 | /24                |
|3        | 172.25.32.3 | /24                |
|4        | 172.25.32.4 | /24                |
