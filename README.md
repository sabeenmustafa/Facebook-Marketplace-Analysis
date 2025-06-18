# 🛒 Facebook Marketplace Revenue Analysis

This project presents a comprehensive data engineering and analytical framework for evaluating and enhancing **Facebook Marketplace's revenue potential** through regional targeting, product category insights, and user behavior modeling. We designed a **relational database**, developed an **ETL pipeline using Talend and PostgreSQL**, and created **interactive Tableau dashboards** to uncover critical business insights.

---

## 📌 Business Context

Facebook Marketplace serves as a dynamic platform for buyers and sellers across the U.S. This project explores how **region-specific product demand** and **user behavior analytics** can optimize **advertising revenue**, helping Facebook deliver more personalized, impactful ad campaigns.

---

## 🎯 Goals

- Identify high-performing **regions** and **product categories**
- Analyze revenue streams based on **user age groups**, **ad types**, and **geography**
- Build a **data warehouse** for analytical processing and OLAP operations
- Support **ad targeting strategy** through behavior-driven segmentation
- Quantify key metrics: Revenue, Profit, Market Cap, Loss, and ROI

---

## 🧩 Key Contributions

- **🔄 Developed ETL pipeline** using **Talend** to integrate structured Marketplace data into **PostgreSQL**
- **📊 Built Tableau dashboards** to visualize regional performance, product trends, and ad effectiveness
- **🤖 Applied machine learning techniques** including:
  - **Collaborative filtering** for personalized recommendation modeling
  - **Clustering** for user segmentation based on purchasing behavior
  - Achieved **95% accuracy** in predicting likely buyer behavior (model logic discussed, code not uploaded)

---

## 🗃️ Datasets Used

- [Facebook Marketplace User & Ad Data](https://www.kaggle.com/datasets/sheenabatra/facebook-data)
- [Facebook Ad Analysis (R)](https://www.kaggle.com/code/chrisbow/an-introduction-to-facebook-ad-analysis-using-r/input)
- [Click Conversion Tracking](https://www.kaggle.com/datasets/loveall/clicks-conversion-tracking)

---

## 🏗️ Database Schema

We designed and implemented a fully normalized **PostgreSQL database schema**. Key tables include:

- `User`, `Buyer`, `Seller`, `Product`, `Category`, `Advertisement`, `Payment`, `Revenue`, `Location`, `Company`, `Access`, `View/Open`

Relational and dimensional models were created, incorporating:

- Slowly Changing Dimensions (SCD Type 1)
- OLAP operations (ROLLUP, DICE, SLICE, etc.)
- Star Schema for Data Warehouse modeling

---

## 🧱 ETL Pipeline

- **Tools Used**: Talend Open Studio, PostgreSQL
- **Data Flow**:
  - Ingest raw Marketplace data (CSV/JSON)
  - Transform data (type conversions, joins, deduplication)
  - Load into PostgreSQL staging and warehouse tables
- **Hierarchies Created**:
  - User (by region and age)
  - Product (by category and brand)
  - Time-based aggregations for revenue analysis

---

## 📈 Analytical Metrics

Key business KPIs evaluated:

| Metric               | Description                                                  |
|----------------------|--------------------------------------------------------------|
| Total Revenue         | Overall income from ads and product transactions            |
| Net Profit Margin     | Efficiency after costs                                       |
| Gross Margin          | Revenue after cost of goods sold                            |
| Market Capitalization | Perceived value based on category, company, region          |
| Total Loss            | Financial risks or ad underperformance                      |
| Advertisement ROI     | Return on investment by ad type and category                |
| Buyer/Seller Split    | Revenue by segment                                          |
| Location Insights     | Performance by region, state, city                          |

---

## 🧠 OLAP Queries (Examples)

- Revenue by product category and region for 2022  
- Gross margin of video ads for electronics  
- Profit by country for clothing ads  
- User count in Boston for 2019  
- Total loss in the U.S. (2019–2021)  

---


## 🧪 Machine Learning Component

While not uploaded in this repo, we also:
- **Built a collaborative filtering model** to recommend products based on past transactions and views
- **Used K-means clustering** to segment users based on demographics and buying activity
- Achieved **95% accuracy** in predicting likely buyer behavior based on historical data

---

## 🛠 Tech Stack

- **ETL**: Talend Open Studio  
- **Database**: PostgreSQL  
- **BI**: Tableau  
- **ML (Offline)**: Python (scikit-learn, pandas)  
- **Modeling**: Star schema, dimensional modeling, SCD

---


