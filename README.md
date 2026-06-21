# 📊 PhonePe Data Analysis Dashboard

An interactive **Power BI Dashboard** built to analyze digital payment transactions, user behavior, transaction success rates, and service-wise performance using a PhonePe-inspired dataset.

The project focuses on transforming raw transactional data into meaningful business insights through KPI tracking, DAX calculations, interactive filters, and executive-level visualizations.

---

## 🚀 Live Dashboard

🔗 **View Dashboard**

https://app.powerbi.com/view?r=eyJrIjoiMWIyYjhkYzgtZjYwNS00NjgwLTkwZDctNTg5N2JkYWNiN2JhIiwidCI6IjE5MjA4NDBiLTA0YjctNDRhZi05YTRkLTk4YmFkZjRlY2M0YSJ9

---

# 📷 Dashboard Preview

![PhonePe Dashboard](https://i.postimg.cc/6QsmZFqV/Dashboard.png)

---

# 🎯 Project Overview

This dashboard provides a comprehensive view of digital payment activities by analyzing:

- Transaction Volume
- Transaction Value
- Registered Users
- Successful Transactions
- Success Rate
- User Demographics
- Payment Status Trends
- Service Performance
- Monthly Growth Trends

The dashboard enables stakeholders to monitor performance, identify trends, and make data-driven decisions.

---

# 📂 Dataset Information

The dataset contains transaction-level information including:

| Field | Description |
|---------|-------------|
| Transaction_ID | Unique transaction identifier |
| User_ID | Unique user identifier |
| Amount | Transaction amount |
| Service | Service category |
| Service Type | Payment method/service type |
| Payment Status | Successful, Failed, Pending |
| Reason | Transaction outcome reason |
| Date | Transaction date |
| Name | Customer name |
| Age | Customer age |
| Age Segment | Boomers, Gen X, Millennials, Gen Z |
| Join Date | User registration date |

---

# 📌 Key Performance Indicators (KPIs)

The dashboard tracks the following business metrics:

### 💳 Total Transactions
Total number of payment transactions processed.

### 💰 Total Transaction Value
Overall monetary value of transactions.

### 👥 Total Users
Distinct users performing transactions.

### ✅ Successful Transactions
Count of successfully completed transactions.

### 🎯 Success Rate
Percentage of successful transactions.

---

# 📈 Month-over-Month (MoM) Analysis

The dashboard includes dynamic growth tracking for:

- Transaction Growth %
- Transaction Value Growth %
- User Growth %
- Successful Transaction Growth %

Using custom DAX calculations.

---

# 📊 Dashboard Features

### Transaction Trend Analysis
- Monthly transaction trends
- Growth monitoring
- Peak transaction periods

### Service Performance Analysis
- Transaction value by service
- Service contribution comparison

### User Demographics
- Users segmented by age group
- Generation-wise distribution

### Payment Status Analysis
- Successful transactions
- Failed transactions
- Pending transactions

### Transaction Pattern Analysis
- Weekday vs Weekend behavior
- Transaction distribution

### Top Users Analysis
- Highest transaction value contributors

---

# 🎛 Interactive Filters

The dashboard includes dynamic slicers for:

- Month
- Age Segment
- Service Type
- Payment Status
- Reason

### Filter Example

![Filters](https://i.postimg.cc/yYtQq2FG/filter.png)

---

# 🛠 Tools & Technologies Used

### Data Visualization
- Power BI Desktop

### Data Transformation
- Power Query

### Data Modeling
- Star Schema Design
- Relationship Management

### DAX Measures
- KPI Calculations
- Growth Metrics
- Previous Month Comparisons
- Success Rate Analysis

---

# 📐 Data Model

The project follows a structured data model consisting of:

### Fact Table
- All_Transactions

### Dimension Tables
- All_Users
- Date_Table

Relationships were created to support efficient filtering and time-intelligence calculations.

---

# 🔥 DAX Highlights

### Total Users

```DAX
Total User =
DISTINCTCOUNT(All_Transactions[User_ID])
```

### Success Rate

```DAX
Success Rate =
DIVIDE(
    [Successfull Transaction],
    [Total_Transaction]
)
```

### Transaction MoM %

```DAX
Total Trans MOM% =
DIVIDE(
    [Total_Transaction] - [Total Transaction Previous Month],
    [Total Transaction Previous Month],
    0
)
```

### Transaction Value MoM %

```DAX
Trans Value MOM% =
DIVIDE(
    [Total_Transaction_Value] - [Transaction value previous month],
    [Transaction value previous month],
    0
)
```

---

# 💡 Business Insights Generated

✔ High transaction success rate (~96%)

✔ Strong month-over-month growth in transaction volume

✔ Growth in transaction value across services

✔ Millennials contribute a significant share of transactions

✔ Weekday transactions dominate overall activity

✔ Service-wise analysis highlights top-performing services

---

# 📁 Repository Structure

```text
phonepe-data-analysis-dashboard
│
├── Dataset/
│   ├── PhonePe Dataset Files
│
├── Phonepay_Dasboard.pbix
│
├── Dashboard.png
│
├── filter.png
│
└── README.md
```

---

# 📬 Connect With Me

If you have suggestions, feedback, or opportunities related to Data Analytics, Business Intelligence, or Power BI, feel free to connect with me.

⭐ If you found this project useful, consider giving it a Star.
