# Bank Offer Insights Dashboard

Welcome to the **Bank Offer Insights Dashboard** project! This repository showcases an interactive Power BI dashboard designed to deliver actionable insights for targeted bank offers—ranging from credit cards to fixed deposits (FDs) and loan products. This project highlights my data analysis, visualization, and business intelligence skills.

---

## Table of Contents
- [Overview](#overview)
- [Data Description](#data-description)
- [Methodology](#methodology)
- [Dashboard Highlights](#dashboard-highlights)
- [Key Insights](#key-insights)
- [Technologies Used](#technologies-used)
- [How to Explore](#how-to-explore)
- [Conclusion](#conclusion)
- [Contact](#contact)

---

## Overview

In this project, I analyzed customer spending and income data from a financial institution to derive insights that help the bank tailor its product offers. The dashboard is divided into sections addressing different product lines:

- **Credit Card Offers:** Analyzing average spend per category, city, occupation, and monthly spending trends.
- **FD & Loan Offers:** Focusing on high-income segmentation, debt-to-income ratios (DTI), and average spend per age group to identify ideal customers for investment and lending products.

The objective is to empower the bank with data-driven decision-making to enhance customer targeting and optimize product offerings.

---

## Data Description

The project uses two main datasets:

- **Customer Spending Data (`cust_spend`):**  
  Contains transaction-level details such as `customer_id`, `month`, `category`, `payment_type`, and `spend`.

- **Customer Details (`cust_details`):**  
  Includes demographic and financial information such as `customer_id`, `age_group`, `city`, `occupation`, `gender`, `marital_status`, and `avg_income`.

These datasets were merged on `customer_id` to compute key metrics like total spend per customer, average spend per category, and income utilization ratios.

---

## Methodology

1. **Data Preparation & Integration**  
   - **Cleaning & Merging:** The data was cleansed (handling missing values and duplicates) and merged using `customer_id` as the key.
   - **Metric Calculation:** Key metrics such as total spend, average spend, and growth rates were computed using Python (Pandas) and DAX in Power BI.

2. **Exploratory Data Analysis (EDA)**  
   - Initial analysis was performed using Python to understand trends and validate assumptions.
   - Basic visualizations were created to identify patterns across spending categories, cities, age groups, and more.

3. **Interactive Dashboard Creation in Power BI**  
   - **Calculated Columns & Measures:** DAX formulas were used to derive KPIs like spending growth rate, income utilization, and DTI.
   - **Slicers & Filters:** Interactive filters (e.g., by location, age group, occupation) allow users to drill down into specific segments.

---

## Dashboard Highlights

### Insights for Credit Card Offers
- **Avg Spend Per Category:**  
  Visualizes customer spending across categories like Travel, Groceries, Electronics, and Apparel.
  
- **Avg Spend Per City & Occupation:**  
  Displays spending variations across major cities (e.g., Mumbai, Delhi NCR, Bengaluru) and across different occupations.
  
- **Spending Growth Rate:**  
  Tracks month-over-month spending growth, enabling targeted credit card rewards or cashback offers.
  
- **Income Utilisation by Payment Type:**  
  Analyzes how different payment methods (UPI, Debit Card, Credit Card) are used.

### Insights for Loans and FD Offers
- **High-Income Segmentation:**  
  Identifies high-income customers (using data-driven thresholds) who are ideal candidates for FD investments.
  
- **Debt-to-Income (DTI) Analysis:**  
  Evaluates DTI ratios across age groups and months to pinpoint customers who may benefit from loan products.
  
- **Avg Spend per Age Group:**  
  Supports segmentation by revealing spending behaviors across various age cohorts.

---

## Key Insights

- **Targeted Product Offering:**  
  - Customers with higher average spend and robust income profiles are ideal for premium credit card and FD offers.  
  - A rising spending trend and high credit card utilization indicate potential for personalized loan products.

- **Regional Differences:**  
  - Cities like Mumbai and Delhi NCR exhibit higher average spends, suggesting a stronger market for high-end financial products.  
  - Location-based insights allow the bank to tailor offers to regional market conditions.

- **Customer Segmentation:**  
  - Age and occupation play critical roles: while younger groups may favor loan products (for education, vehicles, etc.), older segments tend to prefer secure investment options like FDs.

---

## Technologies Used

- **Python:**  
  Data cleaning, processing, and initial exploratory analysis (using Pandas, Numpy, Matplotlib/Seaborn).

- **Power BI:**  
  Creating interactive dashboards and visualizations; using DAX for calculated columns and measures.

- **DAX:**  
  Custom formulas to compute KPIs such as spending growth rate, income utilization, and DTI.

---

## How to Explore

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/BankOfferInsights.git
