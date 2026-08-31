# 🛒 Retail Sales Performance & RFM Customer Segmentation Dashboard


---

## 📊 Executive Summary

* **Business Problem:** Leadership lacked granular visibility into category-level profit margins, seasonal trends, and customer behavioral segments, resulting in unoptimized marketing spend and unmitigated churn risk[cite: 1].
* **Technical Approach:** Processed 10,000 Kaggle retail records in Power BI[cite: 1]. Modeled a custom **RFM (Recency, Frequency, Monetary) Segmentation Table** via DAX[cite: 1] and built core measures for Revenue, Profit, AOV, Total Customers, and Profit Margin % across an executive 3-tab architecture[cite: 1].
* **Strategic Impact:** Identified seasonal sales spikes[cite: 1], mapped dynamic regional revenue rank shifts[cite: 1], pinpointed profit leakage across sub-categories[cite: 1], and isolated high-margin customer cohorts for targeted retention marketing[cite: 1].

---

## 🖼️ Dashboard Architecture

### 📍 Tab 1: Executive Overview
* **KPI Ribbon:** Cards tracking `Total Revenue`, `Total Profit`, `AOV`, `Total Customers`, and `Profit Margin %`[cite: 1].
* **Sales & Profit Trend:** Dual-axis combo line chart mapping `Order Date` hierarchies (Year, Quarter, Month, Day) against Revenue and Profit[cite: 1].
* **Regional Dynamics:** Ribbon chart tracking dynamic yearly rank shifts in total revenue across sales regions[cite: 1].

### 📦 Tab 2: Product Performance
* **Sales vs. Profit Trade-Off:** Area chart comparing `Sub-Category` sales volume directly against net profit[cite: 1].
* **Regional Profitability:** Line chart evaluating category profit variations across geographic regions[cite: 1].
* **Profit Leakage Breakdown:** Waterfall chart displaying step-by-step net profit contribution per sub-category with `Profit Margin %` tooltips to isolate margin erosion[cite: 1].

### 🎯 Tab 3: RFM Customer Segmentation
* **Cohort Revenue Ranking:** Ribbon chart ordering RFM customer segments by overall financial contribution[cite: 1].
* **Margin Split:** Pie chart illustrating the proportional profit margin distribution across RFM tiers[cite: 1].
* **Geospatial Profit Density:** City-level bubble map sizing profit concentration to optimize localized retargeting campaigns[cite: 1].

---

## 🛠️ Data Stack & Key DAX Measures

* **Tools:** Power BI Desktop[cite: 1] | Kaggle Retail Dataset (10,000 Rows)[cite: 1] | DAX Modeling[cite: 1]
* **Core Measures:**
  * **Total Revenue:** `Total Revenue = SUM(Sales)`[cite: 1]
  * **Total Profit:** `Total Profit = SUM(Profit)`[cite: 1]
  * **Profit Margin %:** `Profit Margin % = DIVIDE([Total Profit], [Total Revenue], 0)`[cite: 1]
  * **Average Order Value:** `AOV = DIVIDE([Total Revenue], DISTINCTCOUNT(Order ID), 0)`[cite: 1]

---
