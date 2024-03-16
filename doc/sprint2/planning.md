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

## Building IP Addressing

    Base IP Address: 172.25.32.0 /20

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
| VOIP (67 Nodes)          | 172.25.34.128 | /26                |
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