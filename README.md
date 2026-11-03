# Bank Transactions & Account Holders Analysis

## Project Overview

The **Bank Transactions & Account Holders Analysis** project focuses on exploring banking customer information and transaction records using SQL and MySQL.

The project contains two datasets: Account Holders and Bank Transactions. It aims to understand customer account details, transaction behavior, payment channels, and banking activity through SQL queries.

This project will be further enhanced with Python Exploratory Data Analysis (EDA) and an interactive Power BI dashboard.

## Project Objectives

- Analyze customer account information.
- Explore banking transaction records.
- Understand debit and credit transaction patterns.
- Identify different transaction channels.
- Analyze customer segments and account types.
- Check missing values and duplicate records.
- Generate meaningful insights from banking data.

## Tools & Technologies

| Technology | Purpose |
|---|---|
| MySQL | Database management |
| SQL | Data exploration and analysis |
| CSV | Dataset storage |
| Python | Planned EDA |
| Power BI | Planned dashboard |

## Repository Structure

```text
Bank-Transactions-Analysis/
│
├── Dataset/
│   ├── account_holders.csv
│   └── bank_transactions.csv
│
├── SQL/
│   ├── 01_database_and_tables.sql
│   └── 02_exploratory_data_analysis.sql
│
└── README.md
```

## Database Description

The project contains two main tables.

### 1. account_holders

Stores customer and bank account information.

Important columns:
- account_id
- customer_name
- gender
- date_of_birth
- mobile_number
- email
- city
- state
- account_type
- customer_segment
- branch_name
- ifsc_code
- account_open_date
- initial_deposit
- kyc_status

### 2. bank_transactions

Stores banking transaction information.

Important columns:
- transaction_id
- account_id
- transaction_date
- transaction_type
- transaction_channel
- amount
- merchant_category
- transaction_status
- balance_after_transaction
- branch_name
- description

**Relationship:** The `account_id` column connects the `account_holders` and `bank_transactions` tables using a foreign key.

## SQL Analysis Performed

The current SQL scripts cover:

- Database and table creation.
- Primary key and foreign key constraints.
- Total account and transaction counts.
- Data preview and date range analysis.
- Distinct values in categorical columns.
- NULL and missing-value checks.
- Conditional categorization using CASE WHEN.
- Missing-value handling.
- Branch-wise account distribution.
- Transaction amount statistics.
- Duplicate record checks.

## How to Run the Project

1. Clone or download this repository.
2. Install and open MySQL Workbench.
3. Open `SQL/01_database_and_tables.sql`.
4. Execute the script to create the database and tables.
5. Import `account_holders.csv` into the `account_holders` table.
6. Import `bank_transactions.csv` into the `bank_transactions` table.
7. Open and execute `SQL/02_exploratory_data_analysis.sql`.

**Note:** The database creation script drops and recreates `bank_transactions_db`. Running it again will delete the existing project database and its data.

## Planned Enhancements

### Python EDA
- Data cleaning and preprocessing.
- Missing-value analysis.
- Transaction trend analysis.
- Customer behavior analysis.
- Data visualization using Pandas, Matplotlib and Seaborn.

### Power BI Dashboard
- Total transactions and transaction amount KPIs.
- Debit vs Credit analysis.
- Transaction channel analysis.
- Customer segment analysis.
- Monthly transaction trends.
- Transaction status analysis.
- Interactive filters and visualizations.

## Author

**Vrushali Sathe**



