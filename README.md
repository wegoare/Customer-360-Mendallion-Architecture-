# Customer 360 Analytics using Medallion Architecture

## 📌 Business Problem
Organizations struggle to get a **unified view of customers** due to fragmented data across sales, products, geography, and customer systems.

Business teams need:
- A single source of truth for customer analytics
- Clean, structured, and analytics-ready data
- Insights into customer behavior, revenue, and segmentation

This project solves that problem by building a **Customer 360 data platform** using the **Medallion Architecture**.

---

## 🏗️ Architecture Overview
This project follows a **Bronze → Silver → Gold** architecture:

### 🔹 Bronze Layer (Raw Data)
- Ingests raw CSV files
- No transformations
- Preserves original schema

### 🔹 Silver Layer (Cleaned & Standardized)
- Data type corrections
- Date normalization
- Null handling & deduplication
- Business-ready schemas

### 🔹 Gold Layer (Analytics Layer)
- Star schema (Facts & Dimensions)
- Aggregated metrics
- Customer 360 table for BI consumption

---

## 📂 Datasets Used
- Customers
- Products
- Product Categories & Subcategories
- Sales Transactions (2016–2017)
- Territories

---

## 🧠 Key Gold Tables
- `dim_customers`
- `dim_products`
- `dim_territory`
- `fact_sales`
- `customer_360`

### Customer 360 includes:
- Customer demographics
- Purchase behavior
- Total orders
- Total spend
- Lifetime value indicators

### Pipeline includes:
-<img width="347" height="121" alt="image" src="https://github.com/user-attachments/assets/9765b1bc-9fb2-49c2-ae14-c9cc645e3f14" />

-This can be improved if we use adls gen2 for data storage and pulling the data from there or if you are getting the data from an api 


---

## 📊 Power BI Dashboard
The Power BI report provides:
- Customer segmentation
- Top customers by income and spend
- Sales by geography
- Product performance
- Revenue trends

📌 Features:
- Gender-based color coding
- Interactive slicers
- KPI cards
- Drill-down analytics

- <img width="745" height="361" alt="image" src="https://github.com/user-attachments/assets/3de3dfc1-6142-4a8b-83b9-e06b66173832" />


---

## 🛠️ Tech Stack Used
- **PySpark**
- **Apache Spark**
- **Medallion Architecture**
- **Microsoft Fabric / OneLake**
- **Power BI**
- **Git & GitHub**

---

## 🚀 Key Learnings
- Implemented end-to-end data engineering pipeline
- Applied industry-grade Medallion Architecture
- Built star schema and Customer 360 analytics
- Designed BI-ready datasets
- Created business-focused Power BI dashboards

---

## 📎 How to Run
1. Ingest raw data into Bronze layer
2. Run Silver transformation notebooks
3. Build Gold tables
4. Connect Power BI to Gold tables
5. Explore dashboards

---

## 📬 Contact
**Mayank Gurjar**  
BTech CSE, IIIT Jabalpur  


