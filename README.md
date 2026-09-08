# Customer Churn Analysis

## 📌 Project Overview

This project focuses on analyzing **customer churn, retention, revenue, and customer behavior** for a digital portal.

The analysis combines **SQL and Tableau** to transform customer and transaction data into meaningful business insights. The project explores customer churn patterns, revenue performance, cohort retention, geographic performance, and customer resurrection behavior.

The objective is to provide a comprehensive view of the **customer lifecycle** and identify opportunities to improve customer retention and revenue.

---

## 🎯 Business Objectives

The analysis aims to answer key business questions such as:

* What is the overall customer churn rate?
* How does churn change over time?
* What is the difference between active and passive churn?
* How is revenue changing over time?
* What proportion of revenue comes from new and recurring customers?
* Which countries contribute the most revenue?
* How frequently do customers make purchases?
* How well do different customer cohorts retain over time?
* How many customers return after cancelling their subscription?
* How long does it take customers to return?

---

## 🛠️ Tools & Technologies

* **SQL** – Data extraction, transformation, aggregation, and analysis
* **Tableau** – Interactive dashboards and data visualization
* **Tableau Calculations** – LOD expressions, table calculations, date calculations, and ranking
* **CSV Data** – Source datasets

---

## 📊 Key KPIs

### Customer & Churn Metrics

* Total Customers
* Active Users
* Churned Users
* Churn Rate
* Active Churn Rate
* Passive Churn Rate
* Retention Rate

### Revenue Metrics

* Total Revenue
* Average Order Value (AOV)
* Customer Lifetime Value (LTV)
* New Revenue
* Recurring Revenue
* Revenue by Country

### Customer Behavior Metrics

* Purchases per Customer
* Cohort Retention
* Resurrected Users
* Average Resurrection Time

---

# 🔍 Analysis Performed

## 1. Customer Churn Analysis

Customer churn is analyzed over time to understand customer attrition and identify changes in churn behavior.

The analysis separates churn into:

* **Active Churn**
* **Passive Churn**
* **Overall Churn**

This provides a more detailed understanding of why customers are leaving and helps identify areas where retention strategies can be improved.

---

## 2. Revenue Analysis

Transaction-level data is analyzed to understand revenue performance and customer contribution.

The analysis covers:

* Revenue trends over time
* Revenue by country
* Revenue by subscription type
* New vs. recurring revenue
* Customer-level revenue
* Average Order Value
* Customer Lifetime Value

### Average Order Value

```text
AOV = Total Revenue / Number of Purchases
```

### Customer Lifetime Value

```text
LTV = Total Revenue / Number of Customers
```

---

## 3. New vs. Recurring Customers

The project distinguishes between new and recurring customer activity to understand the contribution of customer acquisition versus existing customer retention to overall revenue.

This helps evaluate the importance of retaining existing customers and generating recurring revenue.

---

# 📈 Cohort Analysis

Cohort analysis is used to understand customer retention over time.

The project includes both:

* **Annual Cohort Analysis**
* **Monthly Cohort Analysis**

Customers are grouped according to their first purchase period, and their subsequent activity is tracked across future periods.

A FIXED LOD calculation is used to identify the customer's first purchase:

```text
{ FIXED [student_id] : MIN([Purchase Date]) }
```

This enables customers to be assigned to their appropriate acquisition cohort and allows retention patterns to be compared across different customer groups.

---

# 🌍 Revenue by Country

Revenue performance is analysed geographically to identify the countries contributing the most to overall revenue.

The analysis includes:

* Revenue by country
* Customer contribution
* Average Order Value
* Top revenue-generating countries

Country-level analysis helps identify high-performing markets and potential opportunities for further growth.

---

# 🔄 User Resurrection Analysis

The project also analyses customers who return after previously cancelling or ending their subscription.

The resurrection analysis examines:

* Total resurrected users
* Average resurrection time
* Original subscription plan
* Resurrected subscription plan
* Original subscription period
* Resurrected subscription period

### Average Resurrection Time

This metric measures the average number of days between the end of a customer's previous subscription and their return.

This analysis can help businesses understand the potential for **re-engaging churned customers**.

---

# 🧮 SQL Analysis

SQL was used as part of the analytical workflow to:

* Extract relevant customer and transaction data
* Join related datasets
* Aggregate customer-level information
* Calculate revenue metrics
* Analyse churn
* Identify customer segments
* Calculate business KPIs
* Support the Tableau dashboards

The SQL queries used for the analysis are available in the `SQL` folder.

---

# 📊 Tableau Dashboards

The project contains multiple Tableau dashboards designed to provide different perspectives of customer and business performance.

### Revenue & Churn

Provides an overview of:

* Revenue performance
* Churn trends
* Subscription behavior
* New and recurring revenue
* Customer activity

### Customer Churn

Provides detailed analysis of:

* Customer churn
* Active vs. passive churn
* Customer behavior
* Churn trends

### Cohort Analysis

Provides:

* Annual cohort retention
* Monthly cohort retention
* Customer behavior across different acquisition cohorts

### Revenue by Country

Provides a geographic view of:

* Revenue contribution
* Country performance
* Top-performing markets

### User Resurrection

Provides insights into:

* Resurrected customers
* Resurrection trends
* Average time to return
* Subscription plan changes

---

# 📁 Repository Structure

```text
customer-churn-analysis/
│
├── README.md
│
├── SQL/
│   └── customer_churn_analysis.sql
│
├── Tableau/
│   └── Dashboard_Customer_churn.twb
│
├── Dashboard/
│   └── customer_churn_dashboard.png
│
└── Data/
    └── README.md
```

---

# 💡 Business Value

The project provides an end-to-end view of the customer lifecycle:

```text
Customer Acquisition
        ↓
First Purchase
        ↓
Recurring Purchases
        ↓
Customer Retention
        ↓
Churn
        ↓
Customer Resurrection
```

By analyzing these stages together, businesses can:

* Identify high-churn customer segments
* Monitor changes in customer retention
* Understand customer purchasing behavior
* Improve recurring revenue
* Identify high-performing geographic markets
* Compare retention across customer cohorts
* Develop strategies to re-engage churned customers

---

# 🚀 Key Takeaways

This project demonstrates an end-to-end **Data Analytics workflow**:

**SQL → Data Analysis → KPI Development → Tableau Calculations → Dashboard Development → Business Insights**

### Skills Demonstrated

* SQL
* Customer Churn Analysis
* Retention Analysis
* Cohort Analysis
* Revenue Analysis
* Customer Segmentation
* Tableau
* Tableau LOD Expressions
* Table Calculations
* Data Visualization
* Dashboard Design
* Business Intelligence
* Data Storytelling

