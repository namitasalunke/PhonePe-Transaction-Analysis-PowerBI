# 📱 PhonePe Transaction Analysis Dashboard | Power BI

## 📌 Project Overview

The **PhonePe Transaction Analysis Dashboard** is an interactive Power BI project developed to analyze digital payment transactions and user activity. The dashboard provides valuable insights into transaction performance, payment success rates, user behavior, service usage, and payment failure analysis through interactive visualizations and KPIs.

This project demonstrates skills in **Power BI, DAX, Data Modeling, Power Query, and Data Visualization**.

---

## 🎯 Objectives

- Analyze overall transaction performance.
- Monitor payment success and failure rates.
- Track monthly transaction trends.
- Analyze registered users and user growth.
- Compare transaction amounts across different services.
- Identify common payment failure reasons.
- Build an interactive dashboard for business decision-making.

---

# 📊 Dashboard Pages

## 🏠 1. Executive Dashboard

### KPIs
- Total Transactions
- Total Transaction Amount
- Registered Users
- Success Rate

### Visuals
- Monthly Transaction Trend
- Transaction Amount by Service
- Payment Status Distribution
- Monthly Transaction Count

---

## 💳 2. Transaction Analysis

### KPIs
- Total Transactions
- Total Transaction Amount
- Average Transaction Value
- Success Rate

### Visuals
- Monthly Transaction Amount
- Monthly Transaction Count
- Transaction Amount by Service
- Payment Status Distribution

---

## 👥 3. User Analysis

### KPIs
- Registered Users
- Total Transactions
- Average Transaction Value
- Success Rate

### Visuals
- Registered Users by Month
- Registered Users by Service
- Registered Users by Service Type
- Monthly Transactions vs Registered Users
- Users by Age

---

## 📈 4. Business Insights & Payment Failure Analysis

### KPIs
- Successful Transactions
- Failed Transactions
- Success Rate
- Failure Rate

### Visuals
- Failed Transactions by Reason
- Payment Status by Service
- Monthly Failed Transactions
- Payment Status Distribution

---

# 📌 KPIs Used

- Total Transactions
- Total Transaction Amount
- Registered Users
- Average Transaction Value
- Successful Transactions
- Failed Transactions
- Success Rate
- Failure Rate

---

# 📐 DAX Measures

```DAX
Total Transactions =
COUNTROWS(All_Transactions)

Total Transaction Amount =
SUM(All_Transactions[Amount])

Average Transaction Value =
DIVIDE(
    [Total Transaction Amount],
    [Total Transactions]
)

Registered Users =
DISTINCTCOUNT(All_Transactions[User_ID])

Successful Transactions =
CALCULATE(
    COUNTROWS(All_Transactions),
    All_Transactions[Payment_Status]="Successful"
)

Failed Transactions =
CALCULATE(
    COUNTROWS(All_Transactions),
    All_Transactions[Payment_Status]="Failed"
)

Success Rate =
DIVIDE(
    [Successful Transactions],
    [Total Transactions],
    0
)

Failure Rate =
DIVIDE(
    [Failed Transactions],
    [Total Transactions],
    0
)
```

---

# 📈 Key Business Insights

- Achieved an overall payment success rate of approximately **96%**, indicating a reliable payment system.
- Payment failures account for a small percentage of total transactions, highlighting stable transaction processing.
- Loan and Money Transfer services contribute significantly to transaction activity.
- Most failed transactions are associated with common issues such as incorrect PIN entries, server errors, and insufficient balance.
- Monthly transaction performance remains consistent throughout the year.
- Interactive filters allow users to analyze performance by month, quarter, service, and service type.

---

# 🛠 Tools & Technologies

- Microsoft Power BI
- DAX (Data Analysis Expressions)
- Power Query
- Microsoft Excel

---

# 📂 Dataset

The dataset includes transaction-level information such as:

- Transaction ID
- User ID
- Date
- Transaction Amount
- Payment Status
- Service
- Service Type
- Failure Reason
- Registered Users

# 🚀 Features

- Interactive dashboard with slicers
- Dynamic KPI cards
- DAX calculations
- Data modeling
- Business insights
- User analysis
- Transaction analysis
- Payment failure analysis
- Professional dashboard design

---

# 💼 Skills Demonstrated

- Power BI Dashboard Development
- Data Cleaning
- Data Modeling
- Power Query
- DAX
- Data Visualization
- Business Intelligence
- Analytical Thinking
- Dashboard Design

---

# 📁 Repository Structure

```
PhonePe-Transaction-Analysis-PowerBI
│
├── README.md
├── PhonePe_Transaction_Analysis.pbix
├── PhonePe_Dashboard.pdf
│
├── Dataset
│   └── PhonePe_Dataset.xlsx
│
└── Dashboard Screenshots
    ├── Executive Dashboard.png
    ├── Transaction Analysis.png
    ├── User Analysis.png
    └── Business Insights.png
```

---

# 👩‍💻 Author

**Namita Pramod Salunke**

**Aspiring Data Analyst**

### Skills
- Power BI
- SQL
- Excel
- Data Visualization
- DAX
- Data Analysis