# 📊 Daily Power BI Practice

This repository contains my daily Power BI practice files. Each day, I explore new features, build dashboards, and improve my data analysis skills using Power BI Desktop.

---

## 🗓️ Daily ##

**What I practiced:**
- Connected Power BI to Excel dataset
- Cleaned raw data using Power Query:
  - Removed null values
  - Renamed inconsistent column headers
  - Changed data types
  - Split columns (e.g., full name into first/last)
  - Replaced values and removed duplicates
- Built a clean data model for future analysis
- Explored different chart types:
  - Clustered bar chart
  - Stacked column chart
  - Line charts
  - Area, stacked area, and 100% stacked area
  - Hierarchy
  - Ribbon chart
  - Waterfall chart
  - Funnel chart
  - Pie chart and Donut chart
  - Donut chart with added URL
  - Treemap chart
  - Treemap chart (another way)
  - Map
  - Filled map
  - Data modeling
  - Gauge
  - KPI
  - Charts
- Customized chart formatting:
  - Changed colors and themes
  - Adjusted data labels and axis titles
  - Modified legend placement
- Applied filters and slicers to make charts interactive
- Created a small dashboard layout combining multiple visuals.

- Creating tables with DAX
  - Bridge table using UNION
  - Calendar table using visuals
  - GROUPBY function
  - SUMMARIZE table
  - SUMMARIZECOLUMNS
  - Custom summary tables like summarize_east, summarize_east2
  - Using FILTER in DAX
 
  ## 🚀 Creating Dashboard Visuals using Measures  

- Built interactive **dashboard visuals** in Power BI.  
- Used **DAX measures** to calculate KPIs and summarize data dynamically.  
- Combined measures with **charts, cards, and slicers** to create meaningful insights.  
- Explored how measures help in **real-time filtering and aggregation** within visuals.  

### 🛠 Key Concepts
- Creating visuals with **Measures instead of calculated columns**.  
- Using measures in **cards, tables, and charts** for dynamic reporting.  
- Understanding the difference between **implicit vs explicit measures**.  

## 🧾 Example Measures  
- DAX
- Total Sales = SUM(Orders[Sales])
- Average Sales = AVERAGE(Orders[Sales])
- Order Count = COUNTROWS(Orders)

*** 📉 Dashboard Highlights
- KPI cards for **Total Sales, Average Sales, and Order Count**  
- Bar/column charts to show **category-wise performance**  
- Slicers for **easy filtering and interactivity**  
- A clean and professional **dashboard layout**

- Implemented **Decomposition Tree** for drill-down analysis.  
- Used **Q&A Visual** for natural language queries.  
- Explored **AI Visuals (Scatter Chart)** for trend insights.  

## 🧮 Created Measures

- DAX
- Grand Total
- grand_total = SUM(Orders[Sales])

- Percent of Total
-  percent_total = 
-  DIVIDE([grand_total], CALCULATE([grand_total], ALL(Orders)))

- Previous Year Total
-  py_total = 
-  CALCULATE([grand_total], SAMEPERIODLASTYEAR(Orders[Order Date]))

- Quarter over Quarter %
-  qoq% =
-  DIVIDE([grand_total] - [py_total], [py_total])

- Year over Year %
-  yoy% =
-  DIVIDE([grand_total] - [py_total], [py_total])

- Selection Total
-  selection_total = 
-  CALCULATE([grand_total], ALLSELECTED(Orders))




## 🛠 Tools Used
- Power BI Desktop

---

## 📌 Note
This is for self-practice and learning purposes. Some data may be sample/dummy.
