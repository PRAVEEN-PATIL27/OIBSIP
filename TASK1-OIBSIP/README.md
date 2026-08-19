# 📊 Retail Sales Exploratory Data Analysis

## 📝 Project Overview

This project was completed as part of the **Oasis Infobyte Data Analytics Internship – Task 1**.

The project focuses on performing **Exploratory Data Analysis (EDA)** on a retail sales dataset to identify meaningful patterns in sales performance, customer demographics, product categories, and seasonal trends.

The analysis uses Python to clean, process, analyze, and visualize the data, followed by actionable business recommendations based on the findings.

\---

## 🎯 Project Objectives

The main objectives of this project are to:

* Analyze overall retail sales performance.
* Identify monthly and quarterly sales trends.
* Analyze customer purchasing behavior based on gender and age groups.
* Identify the best-performing product category.
* Analyze relationships between numerical variables using correlation analysis.
* Generate meaningful business insights and recommendations.

\---

## 🛠️ Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn

\---

## 📂 Dataset Information

The dataset contains retail transaction data with information related to:

* Transaction ID
* Sale Date
* Sale Time
* Customer ID
* Gender
* Age
* Product Category
* Quantity
* Price per Unit
* Cost of Goods Sold (COGS)

The dataset contains **2,000 records** before data cleaning.

\---

## 🔍 Analysis Performed

### 1\. Data Preparation

* Loaded and inspected the dataset.
* Checked dataset dimensions and data types.
* Identified missing values.
* Removed records containing missing values.
* Converted the sale date column into datetime format.

### 2\. Feature Engineering

Additional features were created to support the analysis:

* Total Sales
* Year
* Month
* Month Name
* Quarter

### 3\. Descriptive Statistics

The analysis includes:

* Mean
* Median
* Mode
* Standard Deviation
* Minimum and Maximum values

### 4\. Sales Trend Analysis

* Monthly sales analysis
* Quarterly sales analysis
* Identification of high-performing periods

### 5\. Customer Demographic Analysis

* Sales by Gender
* Transactions by Gender
* Sales by Age Group

### 6\. Product Category Analysis

The performance of the following categories was analyzed:

* Electronics
* Clothing
* Beauty

Metrics analyzed include:

* Total Sales
* Quantity Sold
* Number of Transactions

### 7\. Correlation Analysis

A correlation heatmap was created to analyze relationships between:

* Age
* Quantity
* Price per Unit
* COGS
* Total Sales

### 8\. Additional Analysis

Sales performance was further analyzed by comparing:

* Product Category
* Customer Gender

\---

## 📈 Key Insights

* 💰 **Total Sales:** 908,230
* 🧾 **Total Transactions:** 1,987
* 🏆 **Best Performing Category:** Electronics
* 👥 **Highest Sales Age Group:** 46–55
* 👩 **Highest Sales Gender:** Female
* 📊 **Best Performing Quarter:** Q4 2022 with sales of 208,530
* 📈 **Strongest Correlation with Total Sales:** Price per Unit

\---

## 💡 Business Recommendations

1. **Focus marketing efforts during Q4** as sales performance is strongest during the final quarter.
2. **Target high-value age groups**, particularly customers aged 46–55 and 26–35.
3. **Strengthen the Electronics category** by maintaining product availability and promoting high-performing products.
4. **Improve Beauty category performance** through promotions, bundles, discounts, and targeted marketing.
5. **Use category-specific marketing strategies** based on customer gender and purchasing behavior.

\---

## ⚠️ Dataset Limitations

The dataset contains product categories but does not include individual product names.

Therefore, a **Top 10 Best-Selling Products** analysis could not be performed. Instead, the analysis focuses on product category performance based on total sales, quantity sold, and transaction count.

\---

## 📁 Repository Structure

```text
OIBSIP/
├── Retail\\\_Sales\\\_EDA.ipynb
├── Retail\\\_Sales.csv
└── README.md

```

## 📊 Visualizations Included

The project includes the following visualizations:

* Monthly Sales Trend
* Quarterly Sales Trend
* Total Sales by Gender
* Transactions by Gender
* Sales by Age Group
* Total Sales by Product Category
* Correlation Heatmap
* Sales by Product Category and Gender

\---

## 📌 Conclusion

This exploratory data analysis identified important patterns in retail sales, customer behavior, and product category performance.

The findings show that **Electronics generated the highest revenue**, while **Clothing recorded the highest number of transactions and quantity sold**. Customers aged **46–55** generated the highest sales, and **Q4 2022** was the strongest-performing quarter.

These insights can support better decision-making related to **inventory planning, targeted marketing, customer segmentation, and product category strategy**.

\---

## 👨‍💻 Author

**Praveen Patil**  
Data Analytics Intern | Oasis Infobyte

