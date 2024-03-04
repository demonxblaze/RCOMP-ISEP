# RCOMP 2022-2023 Project - Sprint 1 - Member 1221083 Folder

Within the subject of Redes de Computadores (RCOMP) each group member got a building to work in. In this report, let's work on the cable structured of the Building 1.

Building 1 has the **Data Center** in the room 1.1.4, which means that this room has all the responsibility to connect every building. The **MCC (Main Cross-Connect)** will be connected to the **ICC (Intermediate Cross-Connect)** and connected in the same room to **HCC (Horizontal Cross-Connect)**. The reason for that is the building has a small size and it dont need to cross ICC to every room of the building.

## Standards

### Acess Point

To be able to get WI-FI network on every floor, we have decided to implement Access Points that, individually, cover 15 meters of diameter. The reason is the number of multiple accesses can overload the Access Point.

Since both Floor 0 and Floor 1 has more than 15 meters of diameter. 2 AP will be needed to cover all the space.

### Cables

As defined by the team in the Planning section:

- Copper cables will be **Category 7 (CAT7) Copper Cables**. 
- Fiber cables will be **Optical Fiber Cables**.

The maximum distance of the Copper cables is **90** meters.

### Network Outlets

For each **10** square meters there should be installed **2** Network Outlets. The distance should not exceed **3** meters.

## Campus Backbone

### Measurements

![](Campus_Backbone_Measurements.png)

### Cabling

![](Campus_Backbone_Cabling.png)

## Building 1

### Floor 0

#### Measurements

![](Building_1_Floor_0_Measurements.png)

#### No. of outlets

| Room  | Length (m) | Width (m) | Area (m^2) | No. of outlets |
|-------|------------|-----------|------------|----------------|
| 1.0.1 | 5.2        | 4.9       | 25.5       | 6              |
| 1.0.2 | 3.5        | 4.9       | 17.2       | 4              |
| 1.0.3 | 4.3        | 4.9       | 21.1       | 6              |
| 1.0.4 | 5.0        | 7.1       | 35.5       | 8              |
| 1.0.5 | 5.8        | 4.5       | 26.1       | 6              |
| 1.0.6 | 5.8        | 7.1       | 41.2       | 10             |

#### Cabling

![](Building_1_Floor_0_Cabling.png)

##### Total of outlets

-   40 + 2 (access points)

### Floor 1

#### Measurements

![](Building_1_Floor_1_Measurements.png)

#### No. of outlets

| Room  | Length (m) | Width (m) | Area (m^2) | No. of outlets |
|-------|------------|-----------|------------|----------------|
| 1.1.1 | 3.5        | 7.2       | 25.2       | 6              |
| 1.1.2 | 3.5        | 7.2       | 25.2       | 6              |
| 1.1.3 | 3.5        | 7.2       | 25.2       | 6              |
| 1.1.4 | 7.7        | 7.2       | 55.4       | 12             |
| 1.1.5 | 5.5        | 4.4       | 24.2       | 6              |
| 1.1.6 | 5.8        | 7.2       | 41.7       | 10             |
| 1.1.7 | 5.8        | 4.7       | 27.3       | 6              |

##### Total of outlets

-   52 + 2 (access point)

#### Cabling

![](Building_1_Floor_1_Cabling.png)