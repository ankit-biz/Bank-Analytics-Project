# Bank Analytics Project

## Overview
This project aims to analyze real estate data from India, China, and Russia using MySQL Workbench and Power BI. It focuses on extracting insights from property listings, pricing trends, location-based demand, and market performance to support data-driven decision-making.

![bankdash](https://github.com/user-attachments/assets/4691292f-82c0-41de-9428-b26ad7247fac)


## Features
- **Data Collection**: Importing real estate data from various sources into MySQL.
- **Data Cleaning & Transformation**: Removing duplicates, handling missing values, and normalizing data using SQL queries.
- **Data Modeling**: Designing a relational database schema using SQL.
- **Data Analysis**: Performing queries to analyze price trends, property demand, and regional performance.
- **Visualization**: Creating interactive dashboards in Power BI.

## Technologies Used

- **MySQL**: Used for importing, cleaning, modeling, and querying the data.
- **Power BI**: Used for visualizing the data and creating interactive dashboards.

## Data Sources

The data used in this project is stored across the following CSV files:

1. `account.csv`: Contains information on bank accounts.
2. `card.csv`: Details about the cards issued.
3. `client.csv`: Client details including their birth numbers and districts.
4. `disp.csv`: Information about the account ownership.
5. `district.csv`: Information on the districts, including crime rates, average salary, and more.
6. `loan.csv`: Data related to loans, their amounts, durations, and payment statuses.
7. `order.csv`: Information on the bank transfers.
8. `trnx_19_NEW.csv`, `trnx_20_NEW.csv`, `trnx_21_NEW.csv`: These files contain transaction data for various years.

## Steps in the Project
## Data Processing in MySQL
### 1. Data Import & Preparation
- Created database: `BankAnalytics`
- Created necessary tables (e.g., `district`, `client`, `account`, `loan`, `disp`, `card`, `orders`, `transactions`)
- Loaded data from CSV files using `LOAD DATA INFILE`

### 2. Data Cleaning & Transformation
- Dealt with duplicate values, blank values, NULL values, and corrected data types
- Applied transformations like `ALTER TABLE`, `UPDATE`, and `COALESCE` to standardize data
- Standardized date formats.
- Trimmed unnecessary spaces.

### 3. Data Modeling
- Established relationships using foreign keys.
  ![bank](https://github.com/user-attachments/assets/ee191b44-431e-45d3-91b5-148d2cea92c6)
- Defined primary keys for data integrity.
- Created views and indexes for efficient querying.

### 4. SQL Analysis & Queries
Performed multiple analytical queries, including:
- **Transaction Analysis**
  - Monthly transaction summary.
  - Top 10 customers with the highest transactions.
  - Most common transaction purposes.
- **Loan Analysis**
  - Loan status distribution.
  - District-wise average unpaid loan amounts.
- **Account & Card Analysis**
  - Number of accounts per account type.
  - Distribution of card types among customers.
- **Bank Insights**
  - Number of transactions per bank.
  - Top clients with the highest balance.

### 5. Power BI Dashboard
- Connected MySQL database to Power BI.
   ![Capture](https://github.com/user-attachments/assets/cb58a1f2-18b7-4980-8969-b296db1c288a)
   ![Capture1](https://github.com/user-attachments/assets/6a420bbe-a45e-4e96-b333-075909a6d604)
- Created visualizations for key insights:
  - Transaction trends over time.
  - Customer segmentation based on transaction behavior.
  - Loan repayment status by district.
  - Account type distribution.
  - Bank-wise transaction analysis.

3. **KPIs**: Comparison of previous year vs. current year transaction amounts using **DAX**
4. **No. of Bank Accounts**: Visualized using card data
5. **Top 10 Banks with Maximum Transactions**: Displayed in table format
6. **Types of Cards**: Represented in a **pie chart**
7. **Loan Status Analysis**

## How to Run the Project
1. Install MySQL and import the database using the provided SQL script.

## Conclusion
This project demonstrates how to efficiently analyze banking transactions using SQL and Power BI. It covers **data preparation, advanced SQL queries, and interactive dashboard visualizations** for better financial decision-making.
