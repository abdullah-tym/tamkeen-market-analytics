# 🛒 Tamkeen Market - End-to-End E-Commerce Data Analytics & BI Pipeline

## 📌 Project Overview
An end-to-end data analytics and business intelligence solution for **Tamkeen Market**, an e-commerce platform in Saudi Arabia. 

This project covers the full data lifecycle: initial extraction, cleaning, and feature engineering in **Python**, relational database deployment with **SQLite / SQL**, interactive dashboard design in **Power BI**, and executive pivot modeling in **Excel**.

---

## 🛠️ Complete Project Pipeline & Stack

### 1. Python Data Pipeline (`pandas`, `sqlite3`, `numpy`)
* **Data Cleaning & Handling Nulls:** Filled missing cities with `Unknown` in `customers`, imputed missing brands, and dynamically mapped missing `unit_price` from the product catalog.
* **Feature Engineering:** Calculated exact `net_sales` accounting for discount percentages, and computed `gross_profit` across 180,000+ order item records.
* **Type Conversion & Standardization:** Converted raw datetime strings to `datetime64` types and exported 8 cleaned CSV datasets.
* **Database Deployment:** Programmatically created a `sqlite3` database (`tamkeen_market.db`) and ingested all cleaned relational tables.

### 2. Relational SQL Analysis
* Ran SQL queries directly against SQLite to aggregate executive-level business metrics.
* Evaluated regional performance, monthly sales trends, customer behavior, return reasons, and delivery efficiency across warehouses.

### 3. Power BI Executive Dashboard
* Built a dynamic, multi-visual dashboard featuring DAX measures, custom year filters, regional bar/column performance, category metrics, and marketing channel distribution.

### 4. Excel Business Summary
* Built Pivot Tables and Pivot Charts from cleaned datasets to perform quick validation and regional sales breakdowns.

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

## 📁 Data Model Summary

The project processes 8 core relational entities:
* `customers` (25,000 rows)
* `products` (500 rows)
* `orders` (120,000 rows)
* `order_items` (180,047 rows)
* `deliveries` (120,000 rows)
* `returns` (6,643 rows)
* `warehouses` (5 rows)
* `marketing_channels` (7 rows)
