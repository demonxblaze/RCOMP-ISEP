# RCOMP 2023-2024 Project

- #### Class: 2DJ
- #### Group: 4

# Sprint 3 Planning

## Sprint 3 Backlog

| Task  | Task description                                                                                                                                         |
|-------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| T.3.1 | Update the building1.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building 1. |
| T.3.2 | Update the building2.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building 2. |
| T.3.3 | Update the building3.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building 3. |
| T.3.4 | Update the building4.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building 4  |


## Sprint 3 Task Assignments

**T.3.1** - **1221083**

**T.3.2** - **1220631**

**T.3.4** - **1221276**

## Packet Tracer Simulation

The Packet Tracer simulation will be developed using the following guidelines:
- Version: Packet Tracer 8.2.1.118
- Every building will have a separate Packet Tracer file, that should be named as follows: `buildingN.pkt`, where `N` is the building number.
- All configuration files should be exported as a `.txt` file and stored in the repository.

## OSPF Routing Protocol

#### OSPF Areas
- **OSPF Area 0** will be used as the backbone area.
- **OSPF Area N** will be used as the area for each building, where `N` is the building number.
#### OSPF Process ID
- The OSPF process ID should be **100**.
#### Router ID
- The router id should be **N.N.N.N**, where `N` is the building number.

## HTTP Servers IP Addressing

| Building | IP Address    | Subnet Mask Prefix |
|----------|---------------|--------------------|
| 1        | 172.25.34.2   | /25                |
| 2        | 172.25.38.129 | /26                |
| 3        | 172.25.40.129 | /26                |
| 4        | 172.25.44.129 | /26                |

## VOIP Service Configuration

#### VOIP Numbering Plan
- The IP Phones number should look like **NXXX**, where `N` is the building number and `XXX` is the phone number.

## DNS Configuration

The server previously placed in the DMZ should be configured as a DNS server.
The name of the servers should be ns.rcomp-23-24-2dj-g4 in **Building 1**, and ns.buildingN.rcomp-23-24-2dj-g4 in the other buildings.

#### DNS Domain Names

- The root domain name should be **rcomp-23-24-2dj-g4**, and this will act as the domain name for **Building 1**.
- The other buildings should have a local subdomain named as follows: `buildingN.rcomp-23-24-2dj-g4`, where `N` is the building number.

#### DNS Server IP Addressing

| Building | IP Address    | Subnet Mask Prefix |
|----------|---------------|--------------------|
| 1        | 172.25.34.125 | /25                |
| 2        | 172.25.38.189 | /26                |
| 3        | 172.25.40.189 | /26                |
| 4        | 172.25.44.189 | /26                |