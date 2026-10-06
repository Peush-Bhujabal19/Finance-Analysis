# 📊 Finance Analysis Dashboard | Power BI

<img width="1402" height="742" alt="Screenshot 2026-10-06 162132" src="https://github.com/user-attachments/assets/c9f97a7d-6908-427a-ab61-5c1429ad49c0" />

<img width="1401" height="742" alt="Screenshot 2026-10-06 162152" src="https://github.com/user-attachments/assets/aea117b7-144c-4458-a7e2-a6f903ff9196" />


## 📌 Overview

**Finance Analysis Dashboard** is an end-to-end data analytics project built using **CSV, Power Query, and Microsoft Power BI**.

The objective of this project is to transform raw financial transaction data into a clean, interactive dashboard that helps users understand transaction performance, customer segments, transaction status, fees, taxes, trends, and risk-related information.

The project demonstrates a practical data analyst workflow:

**Raw CSV → Data Cleaning with Power Query → Data Transformation → Data Modeling → DAX/KPIs → Interactive Power BI Dashboard → Business Insights**

---

## 📊 Dataset

The project uses a financial transaction dataset containing **50,069 records and 15 columns**.

### Key Fields

| Column | Description |
|---|---|
| `transaction_id` | Unique transaction identifier |
| `transaction_date` | Date of the transaction |
| `account_id` | Customer account identifier |
| `customer_id` | Customer identifier |
| `transaction_type` | Type of transaction |
| `channel` | Transaction channel such as UPI, ATM, POS, Mobile App, etc. |
| `merchant_category` | Merchant/category associated with the transaction |
| `amount` | Transaction amount |
| `fee_amount` | Fee charged on the transaction |
| `tax_amount` | Tax charged on the transaction |
| `currency` | Transaction currency |
| `transaction_status` | Success, Failed, or Pending |
| `is_fraud` | Fraud indicator |
| `risk_score` | Transaction risk score |
| `reference_no` | Transaction reference number |

### Data Coverage

- **Total raw records:** 50,069
- **Columns:** 15
- **Date range:** 2023–2026
- **Currency:** INR
- **Transaction statuses:** Success, Failed, Pending
- **Fraud indicator:** Yes / No

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI** – Dashboard development and visualization
- **Power Query** – Data cleaning and transformation
- **DAX** – KPI calculations and measures
- **CSV** – Raw data source
- **GitHub** – Project documentation and version control

---

## 🔄 Project Steps

### 1. Load Data

Imported the raw `finance_transactions.csv` file into Power BI.

### 2. Data Cleaning with Power Query

Performed data-quality checks and transformations, including:

- Converted `transaction_date` into a proper date format
- Removed duplicate transaction IDs
- Handled missing values in fee-related fields
- Trimmed leading/trailing spaces from categorical fields
- Standardized inconsistent transaction channel values
- Corrected inconsistent category values
- Checked data types for numeric, text, and date columns
- Validated transaction status and fraud fields
- Prepared the dataset for analysis and reporting

### 3. Data Transformation

Created analysis-ready fields and dimensions required for the dashboard, including:

- Year and month analysis
- Transaction status analysis
- Customer segment analysis
- Gender analysis
- State-wise analysis
- Occupation/category filtering
- Transaction type analysis

### 4. KPI & Measure Creation

Created measures for important business metrics such as:

- Total Amount
- Total Transactions
- Average Transaction Value
- Total Fees
- Total Tax
- Year-over-Year comparison

### 5. Dashboard Development

Built an interactive Power BI report with slicers, KPI cards, charts, tables, and transaction-level details.

---

# 📈 Dashboard

## 1. Overview Analysis

The **Overview Analysis** page provides a high-level summary of financial transaction performance.

### Key KPIs – 2026

| KPI | Value |
|---|---:|
| **Total Amount** | ₹45.32M |
| **Total Transactions** | 4.99K |
| **Average Transaction Value** | ₹9.08K |
| **Total Fees** | ₹75.44K |
| **Total Tax** | ₹13.57K |

### Visualizations Included

- Monthly Total Amount trend
- Transaction Status distribution
- Total Amount by Customer Segment
- Total Amount by State
- Transaction Type Analysis
- Total Amount by Gender
- Dynamic KPI comparison with previous year
- Interactive filters for Year, Metric, Occupation, and Category

### Dashboard Preview

![Finance Analysis - Overview](images/finance-analysis-overview.png)

---

## 2. Transaction Analysis

The **Transactions** page provides detailed transaction-level information for deeper analysis.

### Included Fields

- Transaction ID
- Customer Name
- Transaction Date
- Transaction Type
- Transaction Status
- Gender
- Customer Segment
- State
- Total Amount
- Total Fees
- Total Tax

This page allows users to move from high-level KPIs to individual transaction details, making it easier to investigate specific transactions and identify patterns.

### Dashboard Preview

![Finance Analysis - Transactions](images/finance-analysis-transactions.png)

---

# 💡 Key Results & Insights

Based on the **2026 dashboard view**:

- The dashboard reports approximately **₹45.32M** in total transaction amount.
- Approximately **4.99K transactions** were recorded.
- The average transaction value was approximately **₹9.08K**.
- Total transaction fees were approximately **₹75.44K**.
- Total tax generated was approximately **₹13.57K**.
- **Successful transactions** contributed the majority of transaction value, followed by failed and pending transactions.
- The **Retail** segment contributed the highest transaction amount among the displayed customer segments.
- **Maharashtra** recorded the highest transaction amount among the displayed states.
- **Transfer and Loan EMI** are among the major transaction types by amount.
- The dashboard enables comparison of current-year performance with the previous year using dynamic KPI measures.

> **Note:** Dashboard figures are based on the selected filters and the cleaned Power BI dataset.

---

# 🎯 Business Questions Answered

This dashboard helps answer questions such as:

- What is the total transaction amount?
- How many transactions were processed?
- What is the average transaction value?
- How are transaction amounts changing month by month?
- What percentage/value of transactions are successful, failed, or pending?
- Which customer segments contribute the highest transaction amount?
- Which states generate the highest transaction value?
- Which transaction types contribute the most amount?
- How much revenue is generated through fees and taxes?
- How does the current year's performance compare with the previous year?
- Which transaction and customer dimensions require further investigation?

---

# 📁 Project Structure

```text
Finance-Analysis-PowerBI/
│
├── data/
│   └── finance_transactions.csv
│
├── images/
│   ├── finance-analysis-overview.png
│   └── finance-analysis-transactions.png
│
├── Finance_Analysis.pbix
│
└── README.md
```

---

# ▶️ How to Run

### Step 1 – Clone the Repository

```bash
git clone https://github.com/your-username/Finance-Analysis-PowerBI.git
```

### Step 2 – Open the Project

Open:

```text
Finance_Analysis.pbix
```

using **Microsoft Power BI Desktop**.

### Step 3 – Check the Data Source

If Power BI cannot find the CSV file:

**Home → Transform Data → Data Source Settings → Change Source**

Select:

```text
data/finance_transactions.csv
```

### Step 4 – Refresh the Data

Click:

**Home → Refresh**

Power BI will reload the source data and update the dashboard.

---

# 📌 Skills Demonstrated

This project demonstrates practical skills in:

- Data Cleaning
- Data Transformation
- Power Query
- Power BI
- DAX
- KPI Development
- Data Visualization
- Interactive Dashboard Design
- Business Analysis
- Financial Data Analysis
- Data Quality Checking
- Insight Generation

---

# 👨‍💻 About the Project

This project was created as part of my **Data Analytics portfolio** to demonstrate my ability to take raw transaction data, clean and transform it using Power Query, create analytical measures using DAX, and build an interactive Power BI dashboard for business decision-making.

**Role:** Data Analyst / BI Analyst  
**Tools:** Power BI | Power Query | DAX | CSV  
**Domain:** Finance / Transaction Analytics

---

# ⭐ If You Found This Project Useful

Feel free to **star ⭐ the repository** and explore the dashboard and analysis.
