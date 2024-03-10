# RCOMP 2023-2024 Project - Sprint 1 - Member 1220631 Folder

Within the subject of Redes de Computadores (RCOMP) each group member got a building to work in. In this report, let's work on the cable structured of the Building 2.

## Standards

### Acess Point

In order to provide a WI-FI network on every floor, we have decided to implement **Access Points** that individually cover **30 meters diameter**.

### Cables

As defined by the team in the Planning section:

- Copper cables will be **Category 7 (CAT7) Copper Cables**.
- Fiber cables will be **Monomode Fiber Cables**.

The maximum distance of the Copper cables is **90** meters.

### Network Outlets

For each **10** square meters there should be installed **2** Network Outlets. The distance should not exceed **3** meters.

### Patch Panels

Since all connectors and patch panels should meet the cable specifications and we decided to use CAT7 Cables, all of them are also **CAT7**.
Fiber patch panels to Monomode Optical Fiber should be compatible as well.

### Cross-Connected

Cables connecting an **Intermediate Cross-Connect (ICC)** to a **Horizontal Cross-Connect (HCC)** are limited to **500 meters** long, and cables connecting the **Main Cross-Connect (MCC)** to an **ICC** are limited to **1500 meters** long.

### Copper Patch-Cords

Patch cords go from **0.5 to 5 meters** long. They will be provided to end-users to connect their equipment to outlets.

### Telecommunication Enclosures

Having the number of patch panels we can know the size of our Telecommunication Enclosure. Typical 24 ports CAT7 copper patch panels take **1U**.

**1U** is also added for each corresponding expected switch. And at the end, **100% oversize** must be added.

### Consolidation Point

Since we are using a large set of points of sale, a Consolidation Point must be placed to aggregate a bunch of outlets. In this building, it will be used the **24 ports** Consolidation Points.

## Measurements


### Building 2

#### Floor 0

![](Building_2_Floor_0_Measurements.xlsx)

#### Floor 1

![](Building_2_Floor_1_Measurements.xlsx)

## No. of outlets

### Building 1

#### Floor 0

| Room   | Area (m^2) | No. of outlets |
|--------|------------|----------------|
| 2.0.1  | 19.23      | 4              |
| 2.0.2  | 19.23      | 4              |
| 2.0.3  | 19.23      | 4              |
| 2.0.4  | 19.23      | 4              |
| 2.0.5  | 40.8       | 10             |
| 2.0.6  | 108.3      | 5              |
| 2.0.7  | 108.3      | 5              |
| 2.0.8  | 29.17      | 6              |
| 2.0.9  | 29.17      | 6              |
| 2.0.10 | 8.65       | 4              |
| 2.0.11 | 6.76       | 0              |


#### Floor 1

| Room   | Area (m^2) | No. of outlets |
|--------|------------|----------------|
| 2.1.1  | 26.91      | 6              |
| 2.1.2  | 26.91      | 6              |
| 2.1.3  | 26.91      | 6              |
| 2.1.4  | 26.91      | 6              |
| 2.1.5  | 26.91      | 6              |
| 2.1.6  | 31.83      | 8              |
| 2.1.7  | 31.83      | 8              |
| 2.1.8  | 31.83      | 8              |
| 2.1.9  | 31.83      | 8              |
| 2.1.10 | 31.83      | 8              |
| 2.1.11 | 31.83      | 6              |
| 2.1.12 | 13.84      | 0              |
| 2.1.13 | 31.83      | 8              |
| 2.1.14 | 31.83      | 8              |
| 2.1.15 | 31.83      | 8              |

## Total of outlets

### Building 2

#### Floor 0

-   **52 + 2 (access points)**

#### Floor 1

-   **100 + 3 (access points)**

## Cabling


### Building 2

#### Floor 0

![](Building_2_Floor_0_Cabling.png)

#### Floor 1

![](Building_2_Floor_1_Cabling.png)

## Cable Measurements

### Building 2

#### Floor 0

##### CAT-7 Copper Cables

The order of outlets in relation to cable structure is: ⬇️ - ⬅️ - ➡️ -  ⬆️

**- **From HCC to CP(room 2.0.9):** 5,4 m
- **From CP(room 2.0.9) to Outlets 2.0.10:** 10,8 m + 8,2 m + 7,8 m + 5,2 m = 32 m
- **From CP(room 2.0.9) to Outlets 2.0.9:** 7,2 m + 4,2 m + 1,8 m + 10,8 m + 8,6 m + 5,2 m = 37,8 m
- **From CP(room 2.0.9) to Outlets 2.0.8:** 17,4 m + 15,2 m + 12 m + 15,4 m + 12,2 m + 9,8 m = 82 m

- **From HCC to CP(room 2.0.7):** 13,8 m
- **From CP(room 2.0.7) to AP Outlet (left 2.0.8):** 8,6 m
- **From CP(room 2.0.7) to Outlets 2.0.7:** 2,4 m + 4,4 m + 6,4 m + 8,4 m + 10,4 m = 32 m
- **From CP(room 2.0.7) to Outlets 2.0.6:** 13,2 m + 15,2 m + 17,2 m + 19,2 m + 21,2 m = 86 m
- **From CP(room 2.0.7) to AP Outlet (2.0.6):** 32 m

- **From HCC to CP(room 2.0.5):** 34,6 m
- **From CP(room 2.0.5) to Outlets 2.0.10:** 1,6 m + 6,4 m + 3,2 m + 10,2 m + 8,4 m + 5,2 m + 16,4 m + 7,8 m + 13,2 m + 11 m = 83,4 m
- **From CP(room 2.0.5) to Outlets 2.0.4:** 26,8 m + 20,6 m + 23,8 m + 20 m = 91,2 m

- **From HCC to CP(room 2.0.3):** 55,8 m
- **From CP(room 2.0.3) to Outlets 2.0.3:** 4,4 m + 1,4 m + 5,8 m + 3,2 m = 14,8 m
- **From CP(room 2.0.3) to Outlets 2.0.2:** 12,4 m + 6,6 m + 9,6 m + 5,8 m = 34,4 m
- **From CP(room 2.0.3) to Outlets 2.0.1:** 13,6 m + 10,6 m + 13,4 m + 9,8 m = 47,4 m

**Total Cable Length:** 691,2 m

##### Monomode Optical Fiber Cables

#### First Option ####
- **From MCC to ICC (ICC to outside of building) + (Celing height MCC to floor) + (Building 1 to Building 2):** 12,8 m + 4 m + 40 m = 56,8 m
- **From ICC to HCC:** 0,5 m
- **From ICC to 1st Floor Cable Length:** 0,9 m + 4 m = 4,9 m

#### Second Option ####
- **From MCC to ICC (ICC to outside of building) + (Celing height MCC to floor) + (Building 1 to Building 2):** 12,8 m + 4 m + 663,3 m = 680,1 m

**Total Cable Length:** 742,3 m


#### Floor 1

**The Horizontal Cross-Connect (HCC) and the Consolidation Point (CP) must be placed 1.5 m from the floor. The outlets must be rated 2.5 m from the removable dropped ceiling.**

##### CAT-7 Copper Cables

The order of outlets in relation to cable structure is: ⬇️ - ⬅️ - ➡️ - ⬆️

- **From HCC to CP(room 2.1.11):** 1 m (up) + 2,6 m + 1 m (down) = 4,6 m
- **From CP(room 2.1.11) to AP Outlet (left B.1.11):** 1 m (up) + 9,4 m + 2,5 m (down) = 12,9 m
- **From CP(room 2.1.11) to Outlets 2.1.11:** (6 * 1 m (up) + 6 * 2,5 m (down)) + 7,8 m + 5,8 m + 3,6 m + 2,8 m + 7,8 m + 5,6 m = 54,4 m
- **From CP(room 2.1.11) to Outlets 2.1.10:** (8 * 1 m (up) + 8 * 2,5 m (down)) + 8,6 m + 6,6 m + 5,8 m + 18,4 m + 7,8 m + 15 m + 13 m + 11 m = 114 m
- **From CP(room 2.1.11) to Outlets 2.1.9:** (8 * 1 m (up) + 8 * 2,5 m (down)) + 13,6 m + 11,6 m + 18,2 m + 11 m + 13 m + 20,2 m + 18,2 m + 16,2 m = 150 m

- **From HCC to CP(room 2.1.8):** 1 m (up) + 17,2 m + 1 m (down) = 19,2 m
- **From CP(room 2.1.8) to Outlets 2.1.8:** (8 * 1 m (up) + 8 * 2,5 m (down)) + 3,8 m + 1,8 m + 2,8 m + 15,2 m + 4,8 m + 11,8 m + 9,8 m + 7,8 m = 85,6 m
- **From CP(room 2.1.8) to Outlets 2.1.7:** (8 * 1 m (up) + 8 * 2,5 m (down)) + 10,6 m + 8,6 m + 12,4 m + 7,8 m + 9,8 m + 17 m + 15 m + 13 m = 122,2 m

- **From HCC to CP(room 2.1.6):** 1 m (up) + 27,6 m + 1 m (down) = 29,6 m
- **From CP(room 2.1.6) to Outlets 2.1.6:** (8 * 1 m (up) + 8 * 2,5 m (down)) + 3,8 m + 1,6 m + 2,8 m + 15,2 m + 4,8 m + 11,8 m + 9,8 m + 7,8 m = 85,6 m
- **From CP(room 2.1.6) to Outlets 2.1.5:** (6 * 1 m (up) + 6 * 2,5 m (down)) + 25,8 m + 10,8 m + 23,4 m + 13,2 m + 15,4 m + 18,4 m = 128 m

- **From HCC to CP(room 2.1.4):** 1 m (up) + 46,4 m + 1 m (down) = 48,4 m
- **From CP(room 2.1.4) to Outlets 2.1.4:** (6 * 1 m (up) + 6 * 2,5 m (down)) + 7,2 m + 10,2 m + 4,4 m + 7,8 m + 2 m + 2,8 m = 55,4 m
- **From CP(room 2.1.4) to Outlets 2.1.3:** (6 * 1 m (up) + 6 * 2,5 m (down)) + 14,4 m + 10,8 m + 12,2 m + 8,4 m + 6,2 m + 7 m = 80 m
- **From CP(room 2.1.4) to AP Outlet (down 2.1.3):** 1 m (up) + 12,8 m + 2,5 m (down) = 16,3 m

- **From HCC to CP(room 2.1.2):** 1 m (up) + 54,8 m + 1 m (down) = 56,8 m
- **From CP(room 2.1.2) to Outlets 2.1.2:** (6 * 1 m (up) + 6 * 2,5 m (down)) + 7,2 m + 10,2 m + 4,4 m + 7,8 m + 2 m + 2,8 m = 55,4 m
- **From CP(room 2.1.6) to Outlets 2.1.1:** (6 * 1 m (up) + 6 * 2,5 m (down)) + 14,8 m + 10,8 m + 12,4 m + 8,4 m + 6,2 m + 7 m = 80,6 m
- **From CP(room 2.1.6) to Outlets 2.1.13:** (8 * 1 m (up) + 8 * 2,5 m (down)) + 26,2 m + 28,2 m + 30,2 m + 22,8 m + 20,8 m + 21,6 m + 23,6 m + 25,6 m = 227 m

- **From HCC to CP(room 2.1.14):** 1 m (up) + 79 m + 1 m (down) = 57,4 m
- **From CP(room 2.1.14) to Outlets 2.1.14:** (8 * 1 m (up) + 8 * 2,5 m (down)) + 5 m + 7 m + 9 m + 1,6 m + 11,8 m + 2,8 m + 4,8 m + 6,8 m = 76,8 m
- **From CP(room 2.1.14) to Outlets 2.1.15:** (8 * 1 m (up) + 8 * 2,5 m (down)) + 10 m + 12 m + 14 m + 6,8 m + 4,8 m + 5,6 m + 7,6 m + 9,6 m = 98,4 m
- **From CP(room 2.1.14) to AP Outlet (right 2.1.15):** 1 m (up) + 11,2 m + 2,5 m (down) = 14,7 m

**Total Cable Length:** 1673,3 m

***Monomode Fiber Cable:***

- **From floor cable passageway to HCC:** 1,5 m (to HCC) + 0,9 m = 2,4 m
- **Total Cable Length:** 2,4 m


##### Monomode Optical Fiber Cables

- From **Floor 0** to **MCC** -> **8,0 m**
- From **MCC** to **ICC** -> **1,4 m**
- From **ICC** to **HCC** -> **1,4 m**

## Patch-Cords (0.5 m)

### Building 2

#### Floor 0

-   **54 + 1 (ICC to HCC)**

#### Floor 1

-   **103**

## User-Cords (5 m)

### Building 2

#### Floor 0

-   **54**

#### Floor 1

- **103**

## Patch Panels

### Building 2

#### Floor 0

54 outlets are available on this floor, so a minimum of **3 24 patch panels** (or 5 12 patch panels) are needed. To distribute the patch panels as effective as possible, the following was placed:

- 1 patch panel of 12 ports (HCC);
- 1 patch panel of 12 ports (ICC);
- 1 patch panel of 24 ports (room 2.0.9)
- 1 patch panel of 24 ports (room 2.0.7)
- 1 patch panel of 24 ports (room 2.0.5)
- 1 patch panel of 24 ports (room 2.0.3)

#### Total: **2 patch panels of 12 ports** and **4 patch panels of 24 ports**

#### Floor 1

103 outlets are available on this floor, so a minimum of **5 24-port patch panels** (or 6 12-port patch panels) are needed. To distribute the patch panels as efficient as possible, the following was placed:


- 1 patch panel of 12 ports (HCC);
- 1 patch panel of 24 ports (room 2.1.11)
- 1 patch panel of 24 ports (room 2.1.8)
- 1 patch panel of 24 ports (room 2.1.6)
- 1 patch panel of 24 ports (room 2.1.4)
- 1 patch panel of 24 ports (room 2.1.2)
- 1 patch panel of 24 ports (room 2.1.14)

#### Total: **1 patch panels of 12 ports** and **6 patch panels of 24 ports**


## **Racks** ##

### ***Floor 0:*** ###

For the **HCC** and **ICC:**

- **1U** for 1 copper patch panels of 12 ports (HCC);
- **1U** for 1 fiber patch panel of 12 ports (ICC);
- **1U** expected corresponding switches;
- **3U** an additional 100% over dimensioning.
#### **Total**: 6U


For the four **CP (24 ports):**

- **1U** for 1 copper patch panels of 24 ports;
- **1U** expected corresponding switch;
- **2U** an additional 100% over dimensioning.
#### **Total**: 4U -  use one of the available telecommunications enclosures (6U).



### ***Floor 1*** ###

For the **HCC:**

- **1U** for 1 copper patch panels of 12 ports each (HCC);
- **1U** expected corresponding switches;
- **2U** an additional 100% over dimensioning.
#### **Total**: 4U - use one of the available telecommunications enclosures (6U).

For the six **CP (24 ports):**

- **1U** for 1 copper patch panels of 24 ports;
- **1U** expected corresponding switch;
- **2U** an additional 100% over dimensioning.
#### **Total**: 4U - use one of the available telecommunications enclosures (6U).



## Full Inventory

| Floor     | No. of outlets | CAT-7 Copper Cables (m) | Monomode Fiber Cables (m) | Patch-Cords (0,5 m) | User-Cords (5 m) | Patch panels (12) | Patch panels (24) | Telecommunication Enclosures | AP | CP (24) | CP (12) | Switches |
|-----------|----------------|-------------------------|---------------------------|---------------------|------------------|-------------------|-------------------|------------------------------|----|---------|---------|----------|
| 0         | 54             | 691.2                   | 742.3                     | 55                  | 54               | 2                 | 4                 | 5                            | 2  | 4       | 0       | 5        |
| 1         | 103            | 1673.3                  | 2.4                       | 103                 | 103              | 1                 | 6                 | 7                            | 3  | 6       | 0       | 7        |
| **Total** | 157            | 2364.5                  | 744.7                     | 158                 | 157              | 3                 | 10                | 12                           | 5  | 10      | 0       | 12       |