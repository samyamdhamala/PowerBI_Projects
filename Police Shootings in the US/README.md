# 🚔 Police Shootings Dashboard (2015–2020)  

This project analyzes **U.S. police shooting incidents** from 2015–2020 using Power BI.  
Two datasets (2015–2017 and 2018–2020) were modeled, transformed, and visualized to uncover trends across states, demographics, and suspect circumstances.  

---

## 🔹 Key Features  

### 🗂 Data Preparation  
- Loaded and cleaned two datasets (`2015–2017` and `2018–2020`).  
- Created a calculated `Year` column from the shooting date.  
- Built dedicated **measures tables** for each dataset (`Measures 2015–2017` and `Measures 2018–2020`).  

### 📏 DAX Measures  
- `Shootings` → Count of incidents (`COUNTX`).  
- `ArmedWithGun` → Count of suspects armed with guns (`COUNTX` + `FILTER`).  
- `UnarmedSuspects` → Count of suspects marked as “Unarmed”.  
- `AvrgAge` → Average age of suspects (`AVERAGEX`).  

### 📊 Visualizations  
- **Multi-cards** (Top 3 states) for Shootings, Armed with Gun, Unarmed Suspects, and Average Age.  
- **Clustered Column Chart**: Shootings by year, split by race (Black, Hispanic, Native, White).  
- Consistent design: custom background, shadows, soft corners, and typography.  
- **Duplicated reports** for each time period, allowing side-by-side comparisons.  

---

## 🛠 Skills Demonstrated  
- Power BI data transformation & modeling  
- Advanced DAX (`COUNTX`, `FILTER`, `AVERAGEX`)  
- Dashboard design with professional formatting standards  
- Comparative analysis across multiple time periods  

---

## 📷 Dashboard Preview  

## 2015-2017
<img width="1554" height="739" alt="image" src="https://github.com/user-attachments/assets/b6285f09-35ef-4e42-b4ba-04e8d339b800" />


## 2018-2020
<img width="1560" height="760" alt="image" src="https://github.com/user-attachments/assets/dbf591a1-ca4e-4636-ba06-3377f8029c7b" />


---

✨ This dashboard provides insights into police shootings over two distinct periods, highlighting patterns by **state, race, armament status, and age demographics**.  
