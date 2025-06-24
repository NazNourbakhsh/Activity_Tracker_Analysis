# Activity Tracker Analysis (Power BI Dashboard)

## 📊 Project Overview

In this project, I built a Power BI dashboard to analyze step data by activity type and date. The dataset was provided in Excel and included information on walking and running activities over a 2-week period. The goal was to transform raw data into an insightful, interactive dashboard that monitors trends, performance by day, and weekly behavior patterns.

This project demonstrates my ability to:
- Clean and model data in Power BI
- Build star schema data models
- Create calculated measures using DAX
- Design effective visual dashboards

---

## 🧾 Dataset Information

**Source**: Excel File (`Episode 1 - PersonalPortfolioData.xlsx`)  
**Tables**:
- `FACT_Activity`: Daily step data by activity and date
- `DIM_Activity`: Lookup table for activity types (Running, Walking)
- `DIM_Date`: Calendar table (Date, Day Name, Week of Year)

---

## 🔧 Tools Used

- Microsoft Power BI Desktop
- Microsoft Excel
- DAX (Power BI Calculations)

---

## 🎯 Project Steps

1. **Data Import**:
   - Loaded raw Excel data into Power BI
   - Created 3 separate tables: `FACT_Activity`, `DIM_Activity`, and `DIM_Date`

2. **Data Modeling**:
   - Built a star schema
   - Created relationships:
     - `FACT_Activity[Activity_FK]` → `DIM_Activity[Activity_PK]`
     - `FACT_Activity[Date]` → `DIM_Date[Date]`

3. **DAX Calculations**:
   - `Total Steps`
   - `Average Steps`
   - `% of Total by Activity`
   - Date-level and week-level aggregations

4. **Dashboard Design**:
   - KPI Cards: Total & Average Steps
   - Donut Chart: Total Steps by Activity
   - Bar Charts: Weekly & Daily performance breakdowns
   - Line Chart: Daily step trend with average line
   - Slicers: Activity type, Date

---

## 📈 Dashboard Highlights

- **Dynamic Activity Comparison**: Easily toggle between Walking and Running
- **Time-based Insights**: See how step activity trends by day and week
- **Performance Monitoring**: View total steps and daily averages at a glance
- **Clean Visuals**: Intuitive layout, color-coded metrics, responsive design

![Data Model](screenshots/data_model.png)
![Dashboard](screenshots/dashboard.png)

---

## 📁 Folder Structure
