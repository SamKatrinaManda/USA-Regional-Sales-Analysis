#  USA Regional Sales Analysis (2014–2018)

**End-to-end Exploratory Data Analysis + Interactive Power BI Dashboard**  
Analyzing Acme Co.’s multi-year sales performance across products, channels, customers, and U.S. regions to uncover growth levers and support data-driven decision making.

---

##  Project Overview

This project performs a comprehensive Exploratory Data Analysis (EDA) on Acme Co.’s USA sales data spanning **2014–2018**. The analysis identifies key revenue and profit drivers, seasonal patterns, product and channel performance, regional concentration, customer segmentation, and pricing/margin risks.

The insights were then translated into an interactive **Power BI dashboard** that enables business users to self-serve analysis by time, product, region, and channel.

**Primary Goal:**  
Deliver actionable recommendations for pricing, promotions, channel expansion, and regional investment to drive sustainable growth and reduce concentration risk.

---

##  Business Problem

- Inconsistent revenue and profit performance across U.S. regions  
- Limited visibility into seasonal swings, top-performing SKUs, and channel profitability  
- Difficulty identifying growth opportunities and optimizing resource allocation  
- Need for a single source of truth that supports strategic decision-making

**Core Business Question:**  
*How can we leverage 5 years of historical sales data to pinpoint growth levers across products, channels, and regions and optimize strategy for sustainable growth?*

---

##  Objectives

- Identify top-performing products, channels, and regions driving revenue and profit  
- Uncover seasonal trends and anomalies for better planning  
- Detect pricing and margin risks from outlier transactions  
- Segment customers by revenue vs. profit margin  
- Provide clear recommendations for pricing, promotions, and market expansion  
- Build an interactive dashboard for ongoing self-service analysis

---

##  Dataset Description

**Source:** Multi-sheet Excel workbook (`Regional Sales Dataset.xlsx`)

| Sheet              | Records | Description                                      |
|--------------------|---------|--------------------------------------------------|
| Sales Orders       | 64,104  | Transaction-level sales data (2014–2018)         |
| Customers          | 175     | Customer master data                             |
| Products           | 30      | Product catalog                                  |
| Regions            | 994     | Delivery location details (city, state, lat/lon) |
| State Regions      | 49      | State-to-US-Region mapping                       |
| 2017 Budgets       | 30      | Product-level budget targets for 2017            |

**Key Fields After Processing:**
- Identifiers: `order_number`, `order_date`, `customer_name`, `channel`, `product_name`
- Financials: `quantity`, `unit_price`, `revenue`, `cost`, `profit`, `profit_margin_pct`
- Geography: `state`, `state_name`, `us_region`, `lat`, `lon`
- Time: `order_month_name`, `order_month_num`, `order_month`
- Planning: `budget` (2017)

**Final Cleaned Dataset:** ~64K rows × 21 columns  
*(Exported as `Sales_data(EDA Exported).csv`)*

---

##  Tech Stack

| Category              | Tools / Libraries                          |
|-----------------------|--------------------------------------------|
| Data Manipulation     | Python, Pandas, NumPy                      |
| Visualization         | Matplotlib, Seaborn                        |
| Dashboarding          | Power BI                                   |
| Environment           | Google Colab / Jupyter Notebook            |
| Version Control       | Git + GitHub                               |
