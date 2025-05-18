# 📊 IPL Data Analysis using PySpark

This project demonstrates end-to-end data engineering and analytics using **PySpark**, **SQL**, and basic data visualization tools. It focuses on analyzing IPL (Indian Premier League) match data from two CSV files: `matches.csv` and `deliveries.csv`.

## 🔧 Tech Stack

- **PySpark**: For scalable data transformation and processing  
- **Matplotlib**: For basic data visualizations  
- **Databricks Notebook**: Development environment

## 📂 Dataset Description

- **`matches.csv`**: Contains metadata about each match (e.g., teams, toss winner, match result)  
- **`deliveries.csv`**: Ball-by-ball delivery data with runs, wickets, and player actions

## ✅ Project Workflow

### 1. Schema Definition
- Custom schema was applied using `StructType` for clean and efficient data loading.

### 2. Data Cleaning and Null Handling
- Identified and handled missing/null values in both datasets  
- Explored unique values and ensured data consistency

### 3. Transformations
- Added a new column: `toss impact` → `'Y'` if toss winner == match winner, otherwise `'N'`  
- Calculated toss impact percentage  
- Aggregated top scorers using `groupBy` and `sum(batsman_runs)`  
- Other transformations included:
  - Dismissal types  
  - Extra runs  
  - Over-level summaries  

### 4. Visualizations
Plotted:
- Match result distribution  
- Top 10 batsmen by total runs  
- Toss impact visualizations


## 🧠 Future Improvements

- Build a dashboard using **Tableau** or **Power BI**  
- Incorporate ML models (e.g., player performance prediction)  
- Deploy using **Streamlit** or **Flask** for a web app interface
