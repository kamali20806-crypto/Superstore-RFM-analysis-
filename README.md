# 🛒 Retail Sales Performance & RFM Customer Segmentation Dashboard


---

## 📊 Executive Summary

* **Business Problem:** Leadership lacked granular visibility into category-level profit margins, seasonal trends, and customer behavioral segments, resulting in unoptimized marketing spend and unmitigated churn risk .
* **Technical Approach:** Processed 10,000 Kaggle retail records in Power BI. Modeled a custom **RFM (Recency, Frequency, Monetary) Segmentation Table** via DAX and built core measures for Revenue, Profit, AOV, Total Customers, and Profit Margin % across an executive 3-tab architecture.
* **Strategic Impact:** Identified seasonal sales spikes, mapped dynamic regional revenue rank shifts, pinpointed profit leakage across sub-categories, and isolated high-margin customer cohorts for targeted retention marketing.

---

## 🖼️ Dashboard Architecture

### 📍 Tab 1: Executive Overview
* **KPI Ribbon:** Cards tracking `Total Revenue`, `Total Profit`, `AOV`, `Total Customers`, and `Profit Margin %`.
* **Sales & Profit Trend:** Dual-axis combo line chart mapping `Order Date` hierarchies (Year, Quarter, Month, Day) against Revenue and Profit.
* **Regional Dynamics:** Ribbon chart tracking dynamic yearly rank shifts in total revenue across sales regions.

### 📦 Tab 2: Product Performance
* **Sales vs. Profit Trade-Off:** Area chart comparing `Sub-Category` sales volume directly against net profit.
* **Regional Profitability:** Line chart evaluating category profit variations across geographic regions.
* **Profit Leakage Breakdown:** Waterfall chart displaying step-by-step net profit contribution per sub-category with `Profit Margin %` tooltips to isolate margin erosion.

### 🎯 Tab 3: RFM Customer Segmentation
* **Cohort Revenue Ranking:** Ribbon chart ordering RFM customer segments by overall financial contribution.
* **Margin Split:** Pie chart illustrating the proportional profit margin distribution across RFM tiers.
* **Geospatial Profit Density:** City-level bubble map sizing profit concentration to optimize localized retargeting campaigns.

---

## 🛠️ Data Stack & Key DAX Measures

* **Tools:** Power BI Desktop | Kaggle Retail Dataset (10,000 Rows) | DAX Modeling
* **Core Measures:**
  * **Total Revenue:** `Total Revenue = SUM(Sales)`
  * **Total Profit:** `Total Profit = SUM(Profit)`
  * **Profit Margin %:** `Profit Margin % = DIVIDE([Total Profit], [Total Revenue], 0)`
  * **Average Order Value:** `AOV = DIVIDE([Total Revenue], DISTINCTCOUNT(Order ID), 0)`

---
