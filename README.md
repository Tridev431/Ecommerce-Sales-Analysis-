# Ecommerce-Sales-Analysis-
Interactive Excel Ecommerce Dashboard tracking key operational KPIs, sales trends, and profit margins. Demonstrates end-to-end data cleaning, star-schema data modeling, and interactive visual storytelling. Fully optimized and structured for seamless integration and advanced reporting in Power BI.
# 🛒 Ecommerce Sales Analysis & Profitability Dashboard

## 📌 Project Overview
This project delivers a comprehensive, data-driven analysis of e-commerce business operations, focusing on uncovering critical Key Performance Indicators (KPIs), mapping historical sales trends, and evaluating multi-dimensional profitability. 

Originally architected as an interactive analytical system within Microsoft Excel using advanced data modeling techniques (including Power Pivot, complex DAX expressions, and interconnected Pivot Charts), this project serves as a practical demonstration of end-to-end data pipelines—from raw data ingestion and structural transformation to insightful visual storytelling. 

The underlying analytical engine evaluates a granular dataset containing complete transactional lifecycles, capturing deep operational attributes such as order prioritizing, customer demographic segmentation, precise product taxonomy (categories and sub-categories), geographic distribution, operational shipping metrics, total revenue generation, and net profit margins.

---

## 🎯 Business Problem Statement

### **Background**
The global e-commerce market operates on thin margins where scaling revenue does not automatically guarantee financial sustainability. For a multi-regional e-commerce store operating across diverse product ecosystems (Technology, Office Supplies, and Furniture), maintaining a healthy balance between aggressive promotional discounting and net profitability is a constant operational challenge. 

### **The Core Problem**
While the store successfully generates a massive top-line revenue of **$2.30 Million**, the underlying transactional data reveals critical operational inefficiencies and leakages that drain overall business value:

1. **The Product Profitability Paradox (The Furniture Crisis):** 
   The **Furniture** category acts as a massive revenue driver, bringing in **$741.9K** in sales, yet fails to convert this scale into meaningful bottom-line value, yielding a critically low profit of just **$18.4K**. Even more alarmingly, the **Tables** sub-category is actively bleeding cash, generating a net loss of **-$17,725.48**—making it the single biggest revenue drain in the entire business.
2. **Aggressive Over-Discounting Strategy:** 
   Data insights reveal a deep operational flaw in pricing logic: when **Tables** are sold without discounts, they generate a healthy positive profit of **$13,276**. However, unoptimized promotional strategies and high average discounts ($0.26 per unit) completely erode these margins, resulting in a staggering loss of **-$31,001** on discounted orders.
3. **Regional Conversion Inefficiencies:** 
   Despite solid market penetration across all demographics, the **Central Region** demonstrates severe structural inefficiency. It drives half a million dollars ($501.2K) in sales but fails to retain margins, yielding a mere **$39.7K** in profit—underperforming drastically compared to the highly efficient West and East regions.

### **Objective**
The goal of this interactive dashboard project is to transform raw, fragmented transactional records into actionable, localized insights to help stakeholders optimize discounting thresholds, eliminate bleeding product lines, and re-engineer regional logistics to reclaim lost profit margins.

---

## 🛠️ Technical Toolkit & Architecture
* **Core Dataset:** `Ecommerce Sales Analysis (Recovered).xlsx` (Normalized multi-table layout consisting of 9,994 transactional rows)
* **Data Engineering & ETL:** Power Query (Data cleaning, handling missing records, type casting, and schema optimization)
* **Analytical Modeling:** Power Pivot & Excel Data Model (Establishing star-schema relationships and custom DAX measures)
* **Visualization Layer:** Dynamic Excel Pivot Charts integrated with interactive Slicers and Timelines for seamless filtering
* **Target Migration:** Designed with standard star-schema mappings for immediate import and deployment into **Microsoft Power BI Desktop**.

---

## 📊 Key Insights & Analytical Takeaways

* **Financial Health:** Total Sales reached **$2.30M** with a net profit of **$286.4K**, yielding an overall stable profit margin of **12.47%** across 5,009 unique customer orders.
* **Category Dynamics:** Technology led both Sales ($836.1K) and Profits ($145.4K). Conversely, Furniture generated high sales ($741.9K) but suffered extremely compressed profit margins, returning only $18.4K in total profit.
* **Product Profitability Profit Engines:** Copiers ($55.6K profit), Phones ($44.5K profit), and Accessories ($41.9K profit) emerged as the top 3 profit drivers. 
* **Product Profitability Revenue Drains:** Tables proved to be the most significant drain on revenue, causing a net loss of **-$17.7K**, closely followed by Bookcases (-$3.4K) and generic Supplies (-$1.1K).
* **Geographical Dominance:** The West Region stands out as the most lucrative market, accounting for **$725.4K** in sales and **$108.4K** in net profit, whereas the Central Region requires rapid margin optimization.

---

## 📋 Technical & System Requirements

### 1. Software & Applications
* **Microsoft Excel (2019 or later recommended):** To access the advanced data modeling features, interactive slicers, and Pivot Charts natively inside the workspace.
* **Microsoft Power BI Desktop:** Required if you wish to migrate the existing star-schema data model into a dedicated business intelligence environment for advanced DAX calculation and cloud deployment. 

### 2. Data Infrastructure & Schema
* **Primary Transaction Table (`Data` Sheet):** Requires strict integrity of columns: `Order ID`, `Sales`, `Quantity`, `Discount`, and `Profit`.
* **Date/Time Parsing:** `Order Date` and `Ship Date` must be explicitly configured as standard datetime objects to process temporal trends and compute precise shipping day averages.

---

## 🚀 How to Open and Run the Project

1. **Clone this repository** to your local environment:
```bash
   git clone [https://github.com/Tridev431/Ecommerce-Sales-Analysis-]
