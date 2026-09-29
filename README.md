# Google Fiber Customer Service Analytics Dashboard 📊

## Project Overview
This Business Intelligence (BI) project analyzes customer service call data for "Google Fiber" across multiple markets. The goal is to uncover insights regarding call volumes, repeat call rates, and problem categorization to help management make data-driven decisions and improve customer support efficiency.

The project involves end-to-end data pipeline execution, from raw data extraction and cleaning in **PostgreSQL** to advanced data modeling and visualization in **Power BI**.

---

## 🛠️ Tech Stack & Tools
* **Database & Data Cleaning:** PostgreSQL, pgAdmin 4
* **Business Intelligence:** Microsoft Power BI
* **Data Transformation:** Power Query (ETL)
* **Analytical Language:** DAX (Data Analysis Expressions)

---

## 🔍 Key Features & Analytics

### 1. Data Engineering & Cleaning (PostgreSQL)
* Merged multiple regional market tables using `UNION ALL`.
* Handled missing and null values systematically using `COALESCE(column, 0)` to ensure calculation accuracy.
* Filtered out corrupted records (e.g., missing `date_created`) for a pristine dataset.

### 2. Data Modeling (Power Query)
* Transformed wide data structures into long formats using the **Unpivot** feature to enable dynamic filtering and categorization in Power BI.
* Established properly formatted Date Hierarchies for time-series analysis.

### 3. Advanced DAX Measures
* **Month-over-Month (MoM) Growth:** Time-intelligence functions (`PREVIOUSMONTH`) to track volume changes.
* **Cumulative Running Totals:** `TOTALQTD` for quarter-to-date call accumulation.
* **Pareto Analysis (80/20 Rule):** Identifying the top 20% of problem types causing 80% of repeat calls.
* **Dynamic Top N Slicers:** `RANKX` functions allowing users to dynamically filter top days with the highest call volumes.
* **What-If Parameters:** Interactive simulation to predict total call reduction if Day 1 repeat calls are reduced by a specific percentage.

---

## 📈 Dashboard Previews

### Page 1: Executive Overview
<img width="579" height="324" alt="image" src="https://github.com/user-attachments/assets/d2ccd453-ca11-4b22-a3d4-a87dd5a95f06" />


### Page 2: Market Performance Analysis
<img width="577" height="322" alt="image" src="https://github.com/user-attachments/assets/570e6a60-18f9-44b0-a135-07801681468f" />


### Page 3: Problem Type Deep Dive
<img width="576" height="323" alt="image" src="https://github.com/user-attachments/assets/879bc794-cee5-46d8-8b61-bdccb999babd" />


### Page 4:Analytics & Forecasting
<img width="576" height="322" alt="image" src="https://github.com/user-attachments/assets/cbe04d0c-b6c9-4e79-9819-dbc285666996" />




## 👨‍💻 Author
**Muhammad Saqib**
* Data Analyst | Business Analyst | software engineer
