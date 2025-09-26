# 🍷 Wine Sales & Profits Dashboard  

This project analyzes **wholesale wine sales in England**, focusing on sales performance, profitability, and salesperson contributions.  
The dataset includes customers such as grocery stores, restaurants, and pubs.  

---

## 🔹 Data Modeling  
- Created table relationships for accurate sales and customer analysis.  
- Built a dedicated **“MyMeasures”** table to store all calculated DAX measures.  

---

## 📏 DAX Measures  
- **Total Sales** → `SUMX(Sales, Sales[Cases Sold] * Sales[Price Per Case])`  
- **Total Cost** → `SUMX(Sales, Sales[Cases Sold] * Sales[Cost Price])`  
- **Net Profit** → `[Total Sales] - [Total Cost]`  
- **Sales per Salesperson** → `[Total Sales] / DISTINCTCOUNT(SalespersonID)`  
- Advanced segmentation: Net Profit by customer size (`No. of Stores > 20` vs `< 20`) using `CALCULATE`.  

---

## 📊 Visualizations  

### Sales Report  
- **Map**: Sales by county (bubble size = cases sold).  
- **Line Chart**: Monthly sales trends.  
- **Cards**: Total Cases Sold, Total Sales, Sales per Salesperson.  
- **Tables**: Sales by Year and Quarter.  
- **Salesperson Table**: Performance by first name.  

### Profits Report  
- **Table**: Wine-level sales, total cost, and net profit.  
- **Stacked Column Charts**: Net profit contribution by salesperson and by supplier.  
- **Donut Chart**: Net profit by wine type.  
- **Cards**: Net profit segmented by customer store count (>20 vs <20).  

---

## 🛠 Skills Demonstrated  
- Data modeling & relationship building in Power BI  
- Advanced DAX (`SUMX`, `CALCULATE`, custom KPIs)  
- Dashboard storytelling (maps, line charts, stacked columns, donut charts, cards)  
- Consistent report formatting and usability best practices  

---

## 📷 Dashboard Previews  

<img width="1781" height="899" alt="image" src="https://github.com/user-attachments/assets/3f30c8db-a62d-43fb-bb2b-045673aca3c6" />

<img width="1703" height="898" alt="image" src="https://github.com/user-attachments/assets/0f6b6d1a-4e2b-4c5c-ab62-d00b8b271885" />

<img width="1790" height="900" alt="image" src="https://github.com/user-attachments/assets/342f569d-ca4f-4c86-850c-91a9cd87c627" />


---

✨ This dashboard provides **clear business insights** into wine sales and profitability, enabling stakeholders to evaluate performance across regions, products, and sales teams.  

