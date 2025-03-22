# Bank Loan Analysis Dashboard

Welcome to the **Bank Loan Analysis Dashboard** project! This project showcases how data analytics and visualization techniques can provide actionable insights into bank loan data using SQL and Power BI. The project focuses on analyzing key metrics, identifying trends, and enhancing decision-making for effective loan portfolio management.

---

## 🚀 Project Overview

Banking institutions handle massive amounts of loan data. Proper analysis of this data is essential for risk assessment, customer segmentation, and portfolio optimization. This project tackles these challenges by:

- Extracting and transforming raw data using **SQL queries**.
- Creating insightful **KPIs and metrics** that align with business objectives.
- Visualizing data with an **interactive Power BI dashboard** to enhance decision-making processes.

---

## 📊 Problem Statement

Banking executives often struggle to monitor and evaluate loan performance metrics effectively. This project aims to solve this issue by providing:

1. A comprehensive summary of key loan metrics, including:
   - Total Loan Applications
   - Total Funded Amount
   - Total Amount Received
   - Average Interest Rate
   - Average Debt-to-Income (DTI) Ratio
2. Insights into **good loans vs bad loans** based on loan statuses.
3. Visualization of trends, such as:
   - Monthly Loan Trends
   - Regional Loan Distribution
   - Loan Purpose Breakdown
4. Granular details on individual loan performance for better portfolio tracking.

---

## 🛠️ Tools and Technologies

- **SQL Server**: Used for data storage, cleaning, and querying.
- **Power BI**: For creating interactive dashboards and visualizations.
- **Excel**: For initial data exploration and cross-validation of results.

---

## 📂 Project Structure

### 1. **SQL Analysis**
   - Created a database in SQL Server to store the loan data.
   - Performed data cleaning, transformation, and aggregation using advanced SQL queries.
   - Generated metrics such as:
     - Monthly Loan Applications
     - Good Loan Percentage
     - Funded and Received Amounts by Loan Status
     - Average Interest Rates and DTI
   - Example Query:
     ```sql
     SELECT 
         loan_status, 
         COUNT(id) AS Total_Loans, 
         SUM(loan_amount) AS Total_Funded_Amount, 
         AVG(int_rate) * 100 AS Avg_Interest_Rate 
     FROM 
         bank_loan_data 
     GROUP BY 
         loan_status;
     ```

### 2. **Power BI Dashboard**
   - Imported SQL query results into Power BI.
   - Designed three dashboards:
     1. **Summary Dashboard**: Showcased overall KPIs for loan performance.
     2. **Overview Dashboard**: Highlighted trends across regions, purposes, and time periods.
     3. **Details Dashboard**: Provided granular insights into individual loan metrics.
   - Included filters for dynamic analysis (e.g., by loan grade, region, or purpose).

---

## 📈 Key Features

- **Summary Dashboard**:
  - High-level KPIs such as total loans, funded amount, and average interest rate.
  - Month-over-month (MoM) and year-over-year (YoY) trends.
 
![Summary](Bank_Loan_Analysis/Images/Bank_Loan_Summary.png)
  
- **Overview Dashboard**:
  - Loan trends by issue date, region, term, and borrower profiles.
  - Insights into loan purpose distribution and employment length analysis.
 
![Overview](Bank_Loan_Analysis/Images/Bank_Loan_Overview.png)

- **Details Dashboard**:
  - Detailed loan performance metrics categorized by loan status.
  - Drill-down capabilities for enhanced data exploration.

![Details](Bank_Loan_Analysis/Images/Bank_Loan_Details.png)

---

## 🔍 Insights and Results

1. **Good Loans vs Bad Loans**:
   - Identified the proportion of loans fully paid or current (good loans) vs charged-off loans (bad loans).
   - Suggested strategies to reduce bad loans based on borrower profiles.

2. **Regional Trends**:
   - Highlighted regions with higher default risks and suggested customized lending strategies.

3. **Customer Behavior**:
   - Uncovered key loan purposes and borrower demographics influencing loan performance.

4. **Business Impact**:
   - Provided actionable insights to optimize loan portfolio management, improve cash flow, and reduce risk.

---

## 💡 Learnings and Takeaways

This project demonstrates how to effectively use data analytics and visualization tools to make informed business decisions. By combining **SQL** for data preparation and **Power BI** for visualization, it is possible to deliver impactful insights that drive business growth.

