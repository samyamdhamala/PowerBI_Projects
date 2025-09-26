# 🏟️ Sporting Event Venues Dashboard  

This project analyzes **sporting event venues** by combining event and venue datasets, performing data transformations, and building interactive dashboards in Power BI.  
The reports highlight **venue utilization, heating status, energy costs, and CO₂ emissions** using advanced DAX calculations and R integration for correlation analysis.  

---

## 🔹 Data Modeling  
- Loaded `sporting event venues.xlsx` containing two sheets:  
  - **Event** → Sporting events data (attendance, costs, temperature, etc.).  
  - **Venue** → Venue details (capacity, age, region, etc.).  
- Built a **data model** linking the two tables by the `Venue` field.  
- Renamed tables for clarity: `Event` and `Venue`.  

---

## 📏 Data Transformation & DAX  
- **Event Table**:  
  - `Cost per Attendee` = `(Electricity$ + Natural Gas$) / Average Monthly Attendance` (with `DIVIDE()` handling zeros).  
  - `Heater Status` = `IF(Average Temp < 50, "ON", "OFF")`.  
  - `Utilization` = `Average Monthly Attendance / (RELATED(MaxCapacity) * 1000)` → formatted as % utilization.  

- **Venue Table**:  
  - Split **Venue Capacity** into `MinCapacity (1000)` and `MaxCapacity (1000)`.  
  - Split **Venue Age** into `MinVenueAge` and `MaxVenueAge`.  

---

## 📊 Report Development  

### Utilization Report  
- **Line Chart** → Venue utilization trends.  
- **Stacked Bar Charts** → Event and venue breakdowns.  
- **Table** → Venue details with title “Venue Information”.  

### CO₂ Emissions Report  
- **Scatter Plot**: Utilization (x-axis, no summarization) vs Electricity-related CO₂ emissions (bubble size).  
- **Slicer**: Filter by Venue Region.  
- **R Script Visual**: Correlation Heatmap using `reshape2` and `ggplot2`.  
  - Displays correlation between attendance, temperature, costs, and CO₂ emissions.  
- Added explanatory textbox with notes.  

### Cover Page  
- Textbox with project title, author name, and design elements.  

---

## 🛠 Skills Demonstrated  
- Power BI data modeling & relationships (Excel → Power BI).  
- Advanced DAX (`DIVIDE`, `IF`, `RELATED`).  
- Data cleaning (splitting categorical ranges into numeric fields).  
- Interactive dashboard design with multiple report pages.  
- R integration in Power BI for correlation heatmap visualization.  
- Publishing & sharing reports via **Power BI Service**.  

---

## 📷 Dashboard Previews  
<img width="1481" height="763" alt="image" src="https://github.com/user-attachments/assets/87ccbbc1-3c3e-4202-b216-6f65058a329f" />

<img width="1532" height="776" alt="image" src="https://github.com/user-attachments/assets/a819577f-90eb-42f2-a427-8cc57e907b11" />

<img width="1475" height="775" alt="image" src="https://github.com/user-attachments/assets/a53e4951-0cc1-4885-b685-bdbc60982516" />



---

✨ This dashboard combines **event attendance, venue capacity, and environmental data** to deliver insights into utilization efficiency and sustainability metrics across sporting venues.  
