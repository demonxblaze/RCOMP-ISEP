
# RCOMP 2023-2024 Project - Sprint 1 - Member 1221276 Folder
# T.1.4 - Development of a structured cabling project for building 4.

Within the subject of Redes de Computadores (RCOMP) each group member got a building to work in. In this report, let's work on the cable structured of the Building 4.

## Standards

### Access Point

To be able to get WI-FI network on every floor, we have decided to implement Access Points that, individually, cover 50 meters of diameter.
As walls and other obstacles can reduce this range, we will consider 20-30 meters as the maximum range for each Access Point.

Since the building is about 30 meters long, and 30 meters wide, we would need **3** Access Points on the ground floor. Due to the 
fact that each AP can uphold about 30 users, we will need **4** Access Points in the first floor.

### Cables

As defined by the team in the Planning section:

- Copper cables will be **Category 7 (CAT7) Copper Cables**.
- Fiber cables will be **Monomode Fiber Cables**.

The maximum distance of the Copper cables is **90** meters.

### Network Outlets

For each **10** square meters there should be installed **2** Network Outlets. The distance should not exceed **3** meters.
This rule doesn't apply to rooms 4.0.12, 4.1.19 and 4.1.20, because they are being used as storage rooms, and also to room
4.0.2, because it is a specific purpose room needing only **2** outlets.

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

Since we are using a large set of points of sale, a Consolidation Point must be placed to aggregate a bunch of outlets. 
In this building, we will use **24 ports**, **36 ports** and **48** Consolidation Points.



## Measurements

### Ground Floor
![Building_4_Ground_Floor_Measurements.svg](Building_4_Ground_Floor_Measurements.svg)

    Rooms 4.0.3, 4.0.4, 4.0.5, 4.0.6, 4.0.7, 4.0.8, 4.0.9, 4.0.10 and 4.0.11 are all the same size.

#### No. of outlets


| Room    | Length (m) | Width (m)	  | Area (m^2) | No. of outlets |
|---------|------------|-------------|------------|----------------|
| 4.0.1	  | 5,38	      | 5,38        | 28,94      | 6              |
| 4.0.2   | 	11,54	    | 11,54       | 	133,1716	 | 2              | 
| 4.0.3	  | 6,73       | 	3,2	       | 21,536     | 	6             |    
| 4.0.4   | 	6,73	     | 3,2	        | 21,536     | 	6             |   
| 4.0.5	  | 6,73	      | 3,2	        | 21,536     | 	6             |     
| 4.0.6	  | 6,73	      | 3,2	        | 21,536     | 	6             |     
| 4.0.7	  | 6,73	      | 3,2         | 	21,536    | 	6             |    
| 4.0.8	  | 6,73       | 	3,2        | 	21,536	   | 6              | 
| 4.0.9	  | 6,73       | 	3,2	       | 21,536	    | 6              |
| 4.0.10	 | 6,73       | 	3,2	       | 21,536	    | 6              |
| 4.0.11	 | 6,73       | 	3,2	       | 21,536	    | 6              |
| 4.0.12  | 	3,27	     | 3,85	       | 12,5895	   | 0              |


##### Total Of Outlets

-   68 + 3 (Access Points) = 71

### Floor 1
![Building_4_First_Floor_Measurements.svg](Building_4_First_Floor_Measurements.svg)

    Rooms 4.1.2 and 4.1.3 are the same size.
    Rooms 4.1.4, 4.1.5, 4.1.6, 4.1.7, 4.1.8, 4.1.9, 4.1.10 are all the same size.
    Rooms 4.1.11 and 4.1.12 are the same size.
    Rooms 4.1.13, 4.1.14, 4.1.15, 4.1.16, 4.1.17, 4.1.18 are all the same size.

#### No. of outlets


| Room   | Length (m) | Width (m) | Area (m^2) | No. of outlets |
|--------|------------|-----------|------------|----------------|
| 4.1.1  | 6,92       | 10        | 69,2       | 14             |
| 4.1.2  | 6,15       | 3,85      | 23,68      | 6              |
| 4.1.3  | 6,15       | 3,85      | 23,68      | 6              |
| 4.1.4  | 9,62       | 5,38      | 51,76      | 12             |
| 4.1.5  | 6,73       | 3,85      | 25,91      | 6              |
| 4.1.6  | 6,73       | 3,85      | 25,91      | 6              |
| 4.1.7  | 6,73       | 3,85      | 25,91      | 6              |
| 4.1.8  | 6,73       | 3,85      | 25,91      | 6              |
| 4.1.9  | 6,73       | 3,85      | 25,91      | 6              |
| 4.1.10 | 6,73       | 3,85      | 25,91      | 6              |
| 4.1.11 | 6,15       | 3,85      | 23,68      | 6              |
| 4.1.12 | 6,15       | 3,85      | 23,68      | 6              |
| 4.1.13 | 5,57       | 3,85      | 21,44      | 6              |
| 4.1.14 | 5,57       | 3,85      | 21,44      | 6              |
| 4.1.15 | 5,57       | 3,85      | 21,44      | 6              |
| 4.1.16 | 5,57       | 3,85      | 21,44      | 6              |
| 4.1.17 | 5,57       | 3,85      | 21,44      | 6              |
| 4.1.18 | 5,57       | 3,85      | 21,44      | 6              |
| 4.1.19 | 3,27       | 1,93      | 6,31       | 0              |
| 4.1.20 | 6,35       | 1,93      | 12,26      | 0              |


##### Total of outlets

-   124 + 4 (Access Points) = 128

## Cabling

### Ground Floor
![Building_4_Ground_Floor_Cabling.svg](Building_4_Ground_Floor_Cabling.svg)

### Floor 1
![Building_4_First_Floor_Cabling.svg](Building_4_First_Floor_Cabling.svg)

## Cable Measurements

### Building 4

#### Ground Floor

##### CAT-7 Copper Cables

The order of outlets in relation to cable structure is: ⬇️ - ➡️ - ⬇️ - ⬅️ - ⬅️- ⬇️ - ⬅️ - ⬆️

- From **HCC** to **CP (4.0.3)** -> **42.21 m**
- From **CP (4.0.3)** to **Outlets (4.0.1)** -> 30,78 m + 30,00 m + 29,22 m + 27,97 m + 27,97 + 29,85 m + 30,48 m (AP) = **205,27 m**
- From **CP (4.0.3)** to **Outlets (4.0.2)** -> 12,03 m + 10,93 m = **22,96 m**
- From **CP (4.0.3)** to **Outlets (4.0.3)** -> 5,16 m +4,22 m + 2,66 + 0,31 m + 1,87 m + 2,81 m = **16,03 m**
- From **CP (4.0.3)** to **Outlets (4.0.4)** -> 13,13 m + 12,19 m + 10,78 m + 11,56 m + 12,97 m + 13,91m = **74,54 m**
- From **HCC** to **CP (4.0.6)** -> **29,84 m**
- From **CP (4.0.6)** to **Outlets (4.0.5)** -> 11,51 m + 10,57 m + 9,01 m + 9,94 m + 10,88 m + 11,82 m = **63,83 m**
- From **CP (4.0.6)** to **Outlets (4.0.6)** -> 5,16 m + 4,22 m + 2,66 m + 0,31 m + 1,87 m + 2,81 m + 3,90 m (AP) = **20,93 m**
- From **CP (4.0.6)** to **Outlets (4.0.7)** -> 4,21 m + 3,27 m + 1,4 m + 4,06 m + 5,7 m + 6,64 m = **25,28 m**
- From **HCC** to **CP (4.0.10)** -> **31,72 m**
- From **CP (4.0.10)** to **Outlets (4.0.8)** -> 12,82 m + 11,88 m + 10,52 m + 7,66 m + 9,22 m + 10,16 m = **62,26 m**
- From **CP (4.0.10)** to **Outlets (4.0.9)** -> 9,38 m + 8,44 m 6,88 m + 4,22 m + 5,78 m + 6,72 m = **41,42 m**
- From **CP (4.0.10)** to **Outlets (4.0.10)** -> 5,16 m + 4,22 m + 2,66 m + 0,31 m + 1,87 m + 2,81 m + 3,90 m (AP) = **20,93 m**
- From **CP (4.0.10)** to **Outlets (4.0.11)** -> 3,28 + 2,34 + 0,78 + 3,44 + 4,96 + 5,9 = **20,7 m**
- From **HCC** to **Outlet (4.0.12)** -> **1,56 m (AP)**

##### Monomode Fiber Cables

From **MCC(Building 1)** to **ICC** -> **261,56 m**
From **ICC** to **HCC** -> **1,09 m**

#### Floor 1

##### CAT-7 Copper Cables

The order of outlets in relation to cable structure is: ⬇️ - ➡️ - ⬇️ - ⬅️ - ⬅️- ⬇️ - ⬅️ - ⬆️

- From **HCC** to **CP (4.1.1)** -> **28,28 m**
- From **CP (4.1.1)** to **Outlets (4.1.1)** -> 20,01 m + 19,04 m + 18,13 + 16,25 m + 13,74m + 11,87 m + 9,99 m + 8,11 m + 6,08 m + 3,89 m + 2,95 m + 1,55 m + 1,72 m + 2,97 m = **144,31 m**
- From **CP (4.1.1)** to **Outlet AP** -> **2,19 m**
- From **CP (4.1.1)** to **Outlets (4.1.2)** -> 1,1 m + 2,5 m + 4,06 m + 4,69 m + 5,32 m + 5,95 m = **23,62 m**
- From **CP (4.1.1)** to **Outlets (4.1.3)** -> 7,81 m + 9,69 m + 11,41 m + 12,66 m + 13,44 m + 14,22 m = **69,23 m**
- From **HCC** to **CP (4.1.4)** -> **33,59 m**
- From **CP (4.1.4)** to **Outlet AP** -> **4,38 m**
- From **CP (4.1.4)** to **Outlets (4.1.4)** -> 2,66 m + 4,06 m + 5,31 m + 6,25 m + 7,50 m + 9,06 m + 10,92 + 9,67 m p 8,27 m + 6,82 m + 5,47m + 2,81 m = **73,03 m**
- From **CP (4.1.4)** to **Outlets (4.1.5)** -> 2,65 m + 4,37 m p 6,09 m + 6,72 m + 7,35 m + 7,98 m = **35,16 m**
- From **CP (4.1.4)** to **Outlets (4.1.6)** -> 7,33 m + 9,05 m + 10,77 m + 11,4 m p 12,03 m + 12,66 m = **63,24 m**
- From **HCC** to **CP (4.1.8)** -> **25,47 m**
- From **CP (4.1.8)** to **Outlet AP** -> **3,75 m**
- From **CP (4.1.8)** to **Outlets (4.1.7)** -> 1,4 m + 2,81 m + 4,53 m + 6,09 m + 7,03 m 7,97 m = **29,83 m**
- From **CP (4.1.8)** to **Outlets (4.1.8)** -> 1,72 m + 3,44 m + 5,00 m + 5,78 m + 6,56 m + 7,34 m = **29,84 m**
- From **CP (4.1.8)** to **Outlets (4.1.9)** -> 5,28 m + 7,00 m + 8,56 m + 9,34 m + 10,12 m + 10,9 m = **51,2 m**
- From **CP (4.1.8)** to **Outlets (4.1.10)** -> 10,00 m + 11,72 m + 13,28 m + 14,06 m + 14,84 m + 15,62 m = **79,52 m**
- From **HCC** to **CP (4.1.12)** -> **28,28 m**
- From **CP (4.1.12)** to **Outlets (4.1.11)** -> 2,19 m + 0,94 m + 1,25 m + 1,88 m + 2,82 m + 3,75 m = **12,83 m**
- From **CP (4.1.12)** to **Outlets (4.1.12)** -> 1,56 m p 0,94 m + 2,03 m + 2,81m + 3,59 m + 4,37 m = **15,3 m**
- From **HCC** to **CP (4.1.16)** -> **8,75 m**
- From **CP (4.1.16)** to **Outlet AP** -> **3,75 m**
- From **CP (4.1.16)** to **Outlets (4.1.13)** -> 5,31 m + 6,87 m + 9,21 m + 10,15 m + 11,09 m + 12,03 m = **54,66 m**
- From **CP (4.1.16)** to **Outlets (4.1.14)** -> 11,25 m + 12,03 m + 12,81 m + 13,59 m + 14,37 m + 15,14 m = **79,19 m**
- From **CP (4.1.16)** to **Outlets (4.1.15)** -> 13,65 m + 12,87 m + 12,09 m + 13,03 m + 13,81 m + 14,9 m = **80,35 m**
- From **CP (4.1.16)** to **Outlets (4.1.16)** -> 1,09 m + 2,34 m + 3,59 m + 4,37 m + 5,15 m + 5,93 m = **22,47 m**
- From **CP (4.1.16)** to **Outlets (4.1.17)** -> 1,25 m + 2,81 m + 5,53 m + 5,31 m + 6,09 m + 6,87 m = **27,86 m**
- From **CP (4.1.16)** to **Outlets (4.1.18)** -> 6,25 m + 6,88 m + 7,51 + 8,61 m + 9,39 m + 10,17 m = **49,81 m**

##### Monomode Fiber Cables

From **ICC (Ground Floor)** to **ICC (First Floor)** -> **4,10 m**

## Patch Cords

### Building 4

#### Ground Floor

-   **68 + 3 = 71** patch cords

#### Floor 1
-   **124 + 4 = 128** patch cords

## User Cords (5m)

### Building 4

#### Ground Floor
-   **68** user cords

#### Floor 1
-   **124** user cords

## Patch Panels

### Building 4

#### Ground Floor

71 outlets are available in this floor, so we will need at least **3** 24-port patch panels. Due to needing flexibility 
and scalability we will use **one** 36 port patch panel. With this, our distribution will look like this:

- **1** 12 port patch panel (ICC)
-  **1** 12 port patch panel (HCC)
- **1** 36 port patch panel (CP 4.0.3)
- **1** 24 port patch panel (CP 4.0.6)
- **1** 24 port patch panel (CP 4.0.10)

#### Floor 1

128 outlets are available in this floor, so we will need at least **6** 24-port patch panels. Due to needing flexibility
and scalability we will use **three** 36 port patch panel and one 48 port patch panel. With this, our distribution will look like this:

- **1** 12 port patch panel (HCC)
- **1** 36 port patch panel (CP 4.1.1)
- **1** 36 port patch panel (CP 4.1.4)
- **1** 36 port patch panel (CP 4.1.8)
- **1** 48 port patch panel (CP 4.1.12)

## Telecommunication Enclosures

### Building 4

#### Ground Floor

For the **HCC** and **ICC**:
- **1U** for the copper 12 port patch panel (HCC);
- **1U** for the fiber 12 port patch panel (ICC);
- **2U** For each of the corresponding switches;
- **4U** For a **100%** oversize.

Total: **8U**

For the **CP** in 4.0.3:
- **2U** for the 36 port patch panel;
- **1U** For the corresponding switch;
- **3U** For a **100%** oversize.

Total: **6U**

For the **CP** in 4.0.6:
- **1U** for the 24 port patch panel;
- **1U** For the corresponding switch;
- **2U** For a **100%** oversize.

Total: **4U** - As commercial enclosures start at **6U** we will use a **6U** enclosure.

For the **CP** in 4.0.10:
- **1U** for the 24 port patch panel;
- **1U** For the corresponding switch;
- **2U** For a **100%** oversize.

Total: **4U** - As commercial enclosures start at **6U** we will use a **6U** enclosure.

#### First Floor

For the **HCC**:
- **1U** for the copper 12 port patch panel (HCC);
- **1U** For the corresponding switch;
- **2U** For a **100%** oversize.

Total: **4U** - As commercial enclosures start at **6U** we will use a **6U** enclosure.

For the **CP** in 4.1.1:
- **2U** for the 36 port patch panel;
- **1U** For the corresponding switch;
- **3U** For a **100%** oversize.

Total: **6U**

For the **CP** in 4.1.4:
- **2U** for the 36 port patch panel;
- **1U** For the corresponding switch;
- **3U** For a **100%** oversize.

Total: **6U**

For the **CP** in 4.1.8:
- **2U** for the 36 port patch panel;
- **1U** For the corresponding switch;
- **3U** For a **100%** oversize.

Total: **6U**

For the **CP** in 4.1.12:
- **2U** for the 48 port patch panel;
- **1U** For the corresponding switch;
- **3U** For a **100%** oversize.

Total: **6U**


## Full Inventory

| Floor | No. of outlets | CAT-7 Copper Cables (m) | Monomode Fiber Cables (m) | Patch-Cords (0,5 m) | User-Cords (5 m) | Patch panels (12) | Patch panels (24) | Patch panels (36) | Patch Panels (48) | Telecommunication Enclosures | AP | CP (24) | CP (36) | CP (48) | Switches |
|-------|----------------|-------------------------|---------------------------|---------------------|------------------|-------------------|-------------------|-------------------|-------------------|------------------------------|----|---------|---------|---------|----------|
| 0     | 71             | 648,07                  | 262,65                    | 71                  | 68               | 2                 | 2                 | 1                 | 0                 | 4                            | 3  | 2       | 1       | 0       | 5        |
| 1     | 128            | 1.010,57                | 4,10                      | 128                 | 124              | 1                 | 0                 | 3                 | 1                 | 4                            | 4  | 0       | 3       | 1       | 6        |

