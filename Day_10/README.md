# 🛒 E-Commerce Sales Data Analysis & Profitability Dashboard

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Data_Visualization-yellow.svg)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical_Plots-lightgreen.svg)

## 📌 Project Objective
This project analyzes three years of e-commerce transaction data (2023–2025) to identify top-performing products, visualize revenue trends, and determine how aggressive discounting impacts overall business profitability. By transforming raw transaction logs into dynamic visual dashboards, this project uncovers actionable business intelligence for inventory planning and pricing strategies.

## 📊 Dataset
The data used in this project is sourced from Kaggle. It contains 5,000 detailed e-commerce transactions, including product categories, order dates, regions, sales revenue, applied discounts, and net profit.
* **Dataset Link:** [E-Commerce Sales Dataset by Prince7489](https://www.kaggle.com/datasets/prince7489/e-commerce-sales)

## 🛠️ Tech Stack
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

---

## 🚀 Project Workflow & Key Features

### 1. Data Acquisition & Preprocessing
* Handled missing values (e.g., categorizing blank products as 'Unknown') to preserve data integrity.
* Dropped corrupted rows missing critical financial metrics.
* Converted raw date strings into sortable `datetime` objects for time-series analysis.

### 2. High-Level Business Metrics (EDA)
* Calculated macroscopic performance indicators.
* **Total Sales Revenue:** ₹533,666,024
* **Total Profit:** ₹79,708,734

### 3. Product & Category Performance Dashboard
* Developed horizontal bar charts to rank the **Top 10 Best-Selling Products** by absolute Revenue vs. Volume (Units Sold).
* Created a grouped bar chart to compare Sales vs. Profit across all product categories, highlighting which sectors operate on the thinnest margins.

### 4. Time-Series Analysis (Year-Over-Year Trends)
* Built a 2x2 multi-year dashboard tracking monthly revenue trajectories.
* Extracted specific seasonal peaks for individual years (2023, 2024, 2025) and layered them into a combined YoY comparison chart for management review.

### 5. Metric Correlations
* Generated a Seaborn Heatmap evaluating mathematical relationships between `Quantity`, `Unit Price`, `Discount`, `Sales`, and `Profit` to instantly flag negative financial drivers.

### 6. Profit Drivers & Discounting Impact (Regression Analysis)
* Created a 3x2 matrix of regression plots (`sns.regplot`) to cut through noise and establish mathematical trendlines.
* **Sales vs. Profit:** Filtered out massive 1% wholesale outliers (`Sales < 3000`) to uncover the baseline profitability of core daily orders.
* **Discount vs. Profit:** Utilized `x_jitter` to un-stack fixed discount percentages, visually proving exactly where high discounts drive the company below the zero-profit baseline.

### 7. Geographic Footprint
* Plotted a clean Pie Chart with explosion effects to visualize total sales distribution across geographic regions.

---

## 🎯 Executive Summary & Business Insights
Based on the visual data analysis, we can conclude:
1. **Discounting is Dangerous:** The regression analysis mathematically proves that higher discount tiers aggressively push the company into negative profit margins. The business must restructure its promotional pricing.
2. **Volume ≠ Revenue:** The products that sell the highest number of units are not the products generating the most revenue. Marketing spend should be reallocated toward high-margin, high-revenue items rather than low-value bulk items.
3. **Consistent Seasonality:** The YoY dashboard reveals standard seasonal demand peaks. Supply chain and inventory managers can use this trajectory to forecast warehouse needs for late 2025 and 2026.

---
