# 🛒 E-commerce Sales Data Analytics

## 📌 Project Overview

E-commerce Sales Data Analytics is an end-to-end data analytics project focused on analyzing sales performance, customer behavior, order fulfilment, delivery efficiency, and customer satisfaction for a fictional e-commerce company operating across multiple cities in the United States.

The project uses data cleaning, SQL queries, exploratory analysis, and an interactive dashboard to transform raw transactional data into meaningful business insights.

**Role:** Junior Data Analyst  
**Project Type:** Data Analytics  
**Dataset:** Approximately 5,000 order-item records

---

## 🎯 Business Objectives

The main objectives of this project are:

- Analyze overall sales performance and revenue trends.
- Identify top-performing product categories and customer regions.
- Understand order status and payment method distribution.
- Evaluate delivery performance and identify late deliveries.
- Analyze customer ratings and satisfaction.
- Provide actionable recommendations to improve business operations.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Microsoft Excel | Data cleaning, duplicate removal, standardization, and calculations |
| MySQL | Data storage, SQL queries, and business analysis |
| PowerBI | Dashboard structure | Dashboard styling and layout | Interactive filters, KPIs, and visualizations |

---

## 📂 Project Structure

```text
Ecommerce-Sales-Data-Analytics/
│
├── Ecommerce_Cleaned_Data.csv
│
├── Ecommerce_Sales_Analytics_Dashboard.pbix
│
├── Ecommerce_Sales_Data_Analytics_Project_Report.pdf
│
└── README.md
```

---

## 📊 Dataset Description

The original dataset contains approximately 5,000 order-item records representing e-commerce transactions.

The dataset includes information such as:

- Order ID
- Customer ID
- Customer City
- Customer Region
- Product Category
- Product Name
- Quantity
- Unit Price
- Discount
- Payment Method
- Order Status
- Delivery Partner
- Promised Delivery Date
- Actual Delivery Date
- Customer Review Score

**Data Granularity:** Each row represents an order item. Therefore, distinct order counts are calculated using `COUNT(DISTINCT order_id)` to avoid double-counting orders containing multiple items.

---

## 🧹 Data Cleaning & Preparation

Data cleaning was performed using Microsoft Excel.

Key activities included:

1. Created a working copy of the original dataset.
2. Identified and removed 25 duplicate records.
3. Standardized product categories and payment methods.
4. Handled missing customer city and region values using `Unknown`.
5. Preserved missing delivery dates and review scores rather than assuming values.
6. Created a calculated sales column.

**Calculated Sales Formula:**

```excel
= (Quantity * Unit_Price) - Discount
```

After cleaning, the dataset contained **4,975 records**.

---

## 🗄️ SQL Analysis

MySQL was used to perform business-oriented data analysis.

The analysis covered:

- Total sales and revenue.
- Number of distinct orders.
- Sales by product category.
- Sales by customer region.
- Monthly sales performance.
- Order status distribution.
- Payment method analysis.
- Delivery partner performance.
- Late delivery analysis.
- Customer review analysis.

SQL concepts applied:

- SELECT, WHERE, ORDER BY
- GROUP BY and HAVING
- Aggregate functions
- DISTINCT
- CASE statements
- Date functions
- Subqueries
- Joins (where applicable)

---

## 📈 Key Business Insights

The following are selected findings from the analysis:

| Metric | Result |
|---|---:|
| Cleaned Dataset Records | 4,975 |
| Distinct Orders | 3,599 |
| Delivered Sales | $676,669.26 |
| Average Customer Rating | 3.94 / 5 |
| Late Delivery Rate | 18.40% |
| Cancelled Orders | 145 |
| Cancellation Rate | 4.03% |
| Highest Sales Month | March 2026 |
| March Sales | $81,636.07 |

### Additional Findings

- **Top Product Category:** Electronics
- **Top Customer Region:** Midwest
- **Most Common Order Status:** Delivered
- **Top Payment Method:** UPI / Wallet
- **Sales from UPI / Wallet:** $170,902.18

*Note: Sales figures represent delivered sales where specified. Order-level metrics use distinct order IDs to avoid duplication.*

---

## 📊 Interactive Dashboard

An interactive PowerBI Report.

### Dashboard Features

- Total delivered sales KPI
- Distinct orders KPI
- Average customer rating KPI
- Late delivery rate KPI
- Cancellation rate KPI
- Monthly sales analysis
- Product category performance
- Regional sales analysis
- Order status distribution
- Payment method analysis
- Delivery partner analysis

### Interactive Filters

Users can filter dashboard data by:

- Month
- Customer Region
- Product Category
- Payment Method

Open `Ecommerce_Sales_Analytics_Dashboard.pbix` in a web browser to explore the dashboard.

---

## 💡 Business Recommendations

Based on the analysis, the following recommendations can help improve business performance:

1. **Improve Delivery Efficiency:** Investigate late deliveries and identify operational issues affecting delivery timelines.
2. **Focus on High-Performing Categories:** Monitor Electronics sales and identify opportunities to improve category performance.
3. **Improve Customer Satisfaction:** Analyze lower customer ratings and identify recurring service or product issues.
4. **Reduce Order Cancellations:** Investigate cancellation reasons and improve order fulfilment processes.
5. **Optimize Regional Operations:** Use regional sales performance to support better inventory and marketing decisions.

---

## ⚠️ Project Limitations

- The dataset represents a fictional e-commerce business.
- The analysis is based on the available dataset and its recorded fields.
- Some delivery partner results require reconciliation between the source dataset and SQL aggregation.
- Missing delivery dates and customer reviews were not artificially filled.

---

## 📁 Project Deliverables

- Cleaned e-commerce dataset (`.csv`)
- Interactive analytics dashboard (`.pbix`)
- Detailed project documentation (`.pdf`)
- SQL analysis queries (if included in the repository)

---

## 👨‍💻 Author

**Pramit Kharjule**

Final-Year B.Tech – Electronics and Telecommunication Engineering

MGM College of Engineering, Nanded, Maharashtra, India

- **GitHub:** [github.com/pramit4507](https://github.com/pramit4507)
- **LinkedIn:** [linkedin.com/in/pramit-kharjule-45pk](https://linkedin.com/in/pramit-kharjule-45pk/)

---

## ⭐ Acknowledgement

This project was developed as part of practical learning in Data Analytics, with a focus on applying Excel, SQL, data cleaning, business analysis, and dashboard development to a real-world-style business scenario.

**If you find this project useful, feel free to star the repository!**
