# 📊 Financial Analyst Project – Daily Transaction Data Analysis

This repository contains a complete financial data analysis project performed using **Python**, **Pandas**, **NumPy**, **Matplotlib**, and **Seaborn**.  
The project focuses on **Daily Household Transactions**, including data cleaning, exploratory data analysis (EDA), time-series analysis, category correlations, and visualization of spending patterns.

📄 The full analysis report is available in the PDF file:  
**Financial Analyst Daily Transaction.ipynb – Colab.pdf**

---

## 🔍 Project Overview

The goal of this project is to analyze daily financial transactions and extract insights into spending behavior, trends, and category-wise patterns.  
It covers:

- Data import and basic exploration  
- Handling missing values  
- Data type correction  
- Duplicate removal  
- Summary statistics  
- Transaction trend visualizations  
- Category-wise financial analysis  
- Correlation analysis of spending categories  
- Monthly and daily time-series trends  

---

## 📁 Dataset Description

**Dataset Name:** `Daily Household Transactions.csv`  
**Number of Columns:** 8  
- `Date`  
- `Mode`  
- `Category`  
- `Subcategory`  
- `Note`  
- `Amount`  
- `Income/Expense`  
- `Currency`

**Initial Row Count:** 2461  
**Final Row Count after Cleaning:** 1303  
(1158 rows dropped due to missing dates)

---

## 🛠️ Data Cleaning Steps

### ✔ 1. Missing Value Treatment  
- Dropped rows with missing `Date` (47% of the data)  
- Filled missing values in `Subcategory` and `Note` with `"Unknown"`  

### ✔ 2. Date Conversion  
- Converted the `Date` column to `datetime64[ns]`

### ✔ 3. Duplicate Handling  
- Checked for and removed duplicates (none found)

### ✔ 4. Data Type Verification  
All column data types confirmed appropriate after cleaning.

---

## 📈 Exploratory Data Analysis (EDA)

### **1. Summary Statistics**  
Important highlights:
- **Mean Amount:** 3076.40  
- **Median Amount:** 72.00  
- **Standard Deviation:** 14608.95  
- Amount distribution is **highly right-skewed** with several high-value outliers.

### **2. Visualizations Included**
- Histogram of transaction amounts  
- Box plot (outlier detection)  
- Category-wise transaction counts  
- Income vs Expense distribution  
- Top 3 transaction modes  
- Monthly transaction trends  
- Daily transaction trends  
- Correlation heatmap of spending categories  

---

## 📊 Key Insights

### 🔹 Spending Behavior
- Majority of transactions fall under:
  - **Food**
  - **Transportation**
  - **Household**

- Expenses dominate over income transactions.

### 🔹 Payment Modes
Top 3 modes:
1. Saving Bank Account 1  
2. Cash  
3. Credit Card  

### 🔹 Amount Distribution
- Most transactions are small amounts.
- Few high-value transactions create heavy skewness.

### 🔹 Time-Series Trends
- Monthly spending fluctuates noticeably.
- Daily spending is irregular with sharp spikes.

### 🔹 Category Correlations
- Generated a correlation heatmap of amounts across categories to identify spending patterns.

---

## 📂 Repository Structure

