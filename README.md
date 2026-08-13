# 🛒 Tamkeen Market - End-to-End E-Commerce Data Analytics & BI Pipeline

## 📌 Project Overview
An end-to-end data analytics and business intelligence project for **Tamkeen Market**, an e-commerce platform in Saudi Arabia. 

This project covers the full data lifecycle in a single workflow: raw ETL, data cleaning, feature engineering, and embedded **SQLite / SQL** querying inside **Python (Jupyter Notebook)**, followed by interactive dashboard design in **Power BI** and pivot modeling in **Excel**.

---

## 🛠️ Complete Project Pipeline & Stack

### 1. Python & Embedded SQLite Pipeline (`eda_cleaning.ipynb`)
* **Data Cleaning & Null Imputation:** Handled missing values (filled missing cities with `Unknown` in `customers`, imputed missing brands in `products`, dynamically mapped missing `unit_price` from the catalog, and defaulted missing discounts to 0).
* **Feature Engineering:** Calculated exact `net_sales` (accounting for discount percentages) and `gross_profit` across 180,000+ order item records.
* **Standardization & Clean Export:** Converted date strings to `datetime64` objects and exported 8 cleaned CSV datasets.
* **Embedded SQLite Database:** Created an in-memory/file-based `sqlite3` database directly within the notebook and loaded all 8 cleaned tables.
* **In-Notebook SQL Queries:** Executed SQL queries via `pd.read_sql_query()` to calculate KPIs, monthly revenue trends, city/category performance, return reasons, and delivery efficiency.

### 2. Power BI Executive Dashboard (`tamkeen_dashboard.pbix`)
* Built a dynamic, multi-visual dashboard featuring DAX measures, custom slicers, regional performance, category metrics, and marketing channel distribution.

### 3. Excel Business Summary (`Tamkeen_Market_Analysis.xlsx`)
* Created Pivot Tables and Pivot Charts from cleaned datasets for quick validation and regional sales breakdowns.

---

## 📊 Key Business Metrics (KPIs)

* **Total Revenue:** SAR 36,867,433.62
* **Total Gross Profit:** SAR 10,521,748.12
* **Profit Margin:** 28.54%
* **Total Orders:** 120,000 orders across 25,000 unique customers
* **Average Order Value (AOV):** SAR 307.23
* **Return Rate:** 5.54% (6,643 returns total)
* **Top Market:** **Riyadh** leads with 41,276 orders (SAR 12.65M revenue).
* **Top Category:** **Mobile Accessories** (SAR 6.15M revenue / 57,633 units sold).

---

## 📁 Repository Structure

├── eda_cleaning.ipynb            # Python ETL, Missing Value Handling, & In-Notebook SQLite Queries
├── Tamkeen_Market_Analysis.xlsx  # Excel Pivot Tables & Visuals
├── tamkeen_dashboard.pbix        # Interactive Power BI Dashboard
└── README.md                     # Project Documentation
