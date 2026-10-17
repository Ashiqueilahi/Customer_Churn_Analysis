# Customer Churn Analysis

## Project Overview
Customer Churn Analysis is a data analytics project that analyzes telecom customer data to understand why customers leave a service. The project uses Python for data cleaning and exploratory data analysis, MySQL for querying customer data, and Power BI to build an interactive dashboard.

The goal is to identify customer segments with higher churn rates and provide insights that can help businesses improve customer retention.

## Objectives
- Analyze customer churn and retention rates.
- Clean and preprocess the telecom customer dataset.
- Identify churn patterns based on contract type, tenure, payment method, and internet service.
- Use SQL queries to analyze customer behavior.
- Develop an interactive Power BI dashboard to visualize key performance indicators and trends.

## Dataset
- **Dataset:** Telco Customer Churn
- **Total Records:** 7,043
- **Total Columns:** 21
- **Target Column:** `Churn`
- **Target Values:** Yes (customer churned), No (customer retained)

The dataset contains customer demographics, account information, subscribed services, contract details, payment methods, monthly charges, total charges, and churn status.

## Tools and Technologies
- **Python:** Data cleaning and exploratory data analysis
- **Pandas:** Data manipulation and preprocessing
- **NumPy:** Numerical operations
- **Matplotlib and Seaborn:** Data visualization
- **MySQL:** SQL queries and customer data analysis
- **Power BI:** Interactive dashboards and business reporting

## Project Workflow

### 1. Data Cleaning and Preprocessing
- Loaded the telecom customer dataset using Pandas.
- Checked for missing values and duplicate records.
- Converted `TotalCharges` into a numeric data type.
- Handled 11 missing values in `TotalCharges` by replacing them with 0 after checking the data.
- Verified the cleaned dataset for missing values and duplicates.
- Exported the cleaned dataset for SQL analysis and Power BI visualization.

### 2. Exploratory Data Analysis (EDA)
Analyzed customer churn patterns using visualizations, including:
- Overall churn distribution.
- Churn by contract type.
- Churn by customer tenure.
- Churn by payment method.
- Churn by internet service.
- Monthly charges by churn status.

### 3. SQL Analysis
Used MySQL to perform queries and analyze:
- Overall customer churn rate.
- Churn by contract type.
- Churn by payment method.
- Churn by tenure groups.
- Monthly charges by churn status.
- Churn by internet service.
- Churn by gender and senior citizen status.

### 4. Power BI Dashboard
Developed an interactive dashboard with two pages.

**Page 1: Customer Churn Overview**
- Total Customers
- Churned Customers
- Churn Rate
- Churn by Contract Type
- Churn by Tenure
- Churn by Payment Method
- Churn by Internet Service
- Interactive slicers for contract, senior citizen status, and internet service

**Page 2: Churn Insights and Trends**
- Churn Rate by Contract Type
- Churn Rate by Payment Method
- Churn Rate by Internet Service
- Churn Rate by Tenure Group
- Customer churn and retention KPI cards
- Business insights summary

## Key Findings
- **Total Customers:** 7,043
- **Churned Customers:** 1,869
- **Retained Customers:** 5,174
- **Overall Churn Rate:** 26.54%
- **Retention Rate:** 73.46%

Additional analysis compares churn rates across contract types, payment methods, internet services, and tenure groups to identify customer segments that may need retention-focused strategies.

## Business Recommendations
- Review month-to-month contracts to understand why customers leave.
- Develop retention strategies for customers in their early months of service.
- Investigate customer feedback and service issues among high-churn segments.
- Evaluate payment methods and service offerings associated with higher churn.
- Monitor churn and retention KPIs regularly using the Power BI dashboard.

## Project Structure

Customer-Churn-Analysis/
│
├── Telco-Customer-Churn-Cleaned.csv
├── Customer_Churn_Analysis.ipynb
├── Customer_Churn_Analysis.pbix
└── README.md

## How to Run the Project

### Python Analysis
1. Clone or download this repository.
2. Install the required Python libraries:

   pip install pandas numpy matplotlib seaborn

3. Open `Customer_Churn_Analysis.ipynb` in Jupyter Notebook or Google Colab.
4. Update the dataset path if necessary.
5. Run the notebook cells.

### SQL Analysis
1. Open MySQL Workbench.
2. Create a database named `customer_churn`.
3. Import the cleaned CSV dataset into MySQL.
4. Run the SQL queries to reproduce the analysis.

### Power BI Dashboard
1. Open `Customer_Churn_Analysis.pbix` in Power BI Desktop.
2. Update the dataset path if necessary.
3. Refresh the data.
4. Explore the dashboard using the charts and slicers.

## Skills Demonstrated
- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- SQL Querying
- Data Visualization
- KPI Development
- Power BI Dashboard Development
- Business Insights and Reporting

## Conclusion
This project demonstrates an end-to-end data analytics workflow using Python, MySQL, and Power BI. It transforms raw telecom customer data into meaningful insights that help businesses understand churn patterns and make informed customer retention decisions.
