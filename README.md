## 1.	Project Title / Headline 📑
Sales Analytics Overview: End-to-End Microsoft Fabric & Power BI Sales Insights Dashboard

## 2. Short Description / Purpose 🎯
The Sales Analytics Overview dashboard is an interactive Power BI report backed by a Microsoft Fabric data pipeline, Lakehouse, and Data Warehouse. It provides business leaders, sales managers, and data analysts with real-time visibility into ₹13.64M ($164.38K USD) in total revenue across 1,268 orders and 10,043 units sold, enabling data-driven decisions around regional growth, inventory allocation, and key account retention.

## 3. Tech Stack 💻  
The dashboard was built using the following tools and technologies:  
- Microsoft Fabric Data Pipelines  – Orchestrates automated end-to-end ingestion, notebook transformations, and warehouse loading.
- Microsoft Fabric Lakehouse  – Stores raw CSV files (Files/raw) and Delta tables across a Medallion architecture (bronze_sales, silver_sales, and gold_sales_summary).
- Fabric Notebooks (PySpark / Spark SQL) – Executes ETL logic across pipeline stages (copydatatodelta, TransformBronzeToSilver, BuildGoldLayer).
- Microsoft Fabric Data Warehouse  – Formated the curated star schema (fact_sales, dim_customer, dim_date, dim_product, dim_region) for analytical querying.
- Power BI Semantic Model & DAX – Connects the warehouse tables to the reporting layer with calculated measures.
- Power BI  – Main interactive visualization and reporting interface.

## 4. Features / Highlights:
### 📌 Business Problem
Sales and operations teams often struggle to consolidate raw transactional logs into actionable insights across regions, product lines, and time periods. Answering critical operational questions—such as Which regions drive the highest revenue? How do order counts compare against revenue across product categories? Who are our highest-value customers?—is slow and error-prone without an automated pipeline and unified reporting layer.  
### 📌 Goal of the Dashboard
The primary goal of this dashboard is to deliver an automated, interactive analytical solution that can eliminate the need of uploading data manually,track top line revenue and enables leaders to track the performance.
### 📌 Walkthrough of Key Visuals
* Interactive Time Slicers : Dropdown filters for Date, Month, Quarter, and Year allow users to dynamically filter every KPI and chart on the report.
* KPI Cards : Total Revenue (₹13.64M), Total Revenue in USD ($164.38K), Total Orders (1,268), Total Quantity Sold (10,043), Avg Revenue Per Order (₹10.76K), Avg Quantity Per Order (8.03 units).
* Monthly Revenue & Orders Trend ( Bar & Line Chart): Tracks monthly revenue against total order volume from January to December, highlighting peak sales in October (₹1.4M) and seasonal dips in September (₹0.9M).
* Orders By Product Category (Donut Chart): Shows an even distribution of order volume across Electronics, Furniture and Office Supplies.
* Total Revenue By Category (Column Chart): Contrasts revenue contribution by category, revealing that Electronics dominates revenue at ₹9.04M, followed by Furniture (₹3.80M) and Office Supplies (₹0.80M).
* Quantity Sold By Product Category (Donut Chart): Highlights unit volume distribution, where Office Supplies leads with 7.03K units compared to Furniture and Electronics.
* Revenue & Orders By Region (Horizontal Bar Charts): Compares regional performance across North, West, East, and South, showing North and West tied for top revenue and North leading in order volume.
* Top 10 Customers By Revenue (Ranked Table): Lists the highest-spending customers.
### 📌 Business Impacts & Insights
* Regional Resource Allocation: With North and West generating ₹3.61M each and South trailing at ₹2.95M, sales teams can investigate promotional gaps in the South region while maintaining fulfillment capacity in the North.
* Customer Retention: Identifying the top 10 revenue-generating customers enables targeted loyalty programs and proactive account management for high-frequency buyers.
* Automated Data Reliability: Leveraging a Medallion Lakehouse and Data Warehouse architecture ensures single-source-of-truth reporting with minimal manual intervention.
