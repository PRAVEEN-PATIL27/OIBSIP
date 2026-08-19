````markdown
# 👥 Customer Segmentation Analysis

## 📝 Project Overview

This project was completed as part of the **Oasis Infobyte Data Analytics Internship – Task 2**.

The objective of this project is to segment an e-commerce company's customers into distinct groups based on their purchasing behaviour. The analysis uses **RFM (Recency, Frequency, Monetary) analysis** and **K-Means clustering** to identify meaningful customer segments and provide targeted marketing recommendations.

---

## 🎯 Project Objectives

The main objectives of this project are to:

- Analyze customer purchasing behaviour.
- Calculate customer-level metrics such as purchase frequency, average purchase value, and customer lifetime value.
- Perform RFM analysis using Recency, Frequency, and Monetary features.
- Standardize customer behaviour data using `StandardScaler`.
- Apply the K-Means clustering algorithm to segment customers.
- Use the Elbow Method to determine an appropriate number of clusters.
- Profile each customer segment based on purchasing behaviour.
- Provide targeted marketing recommendations for each customer segment.

---

## 🛠️ Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## 📂 Dataset Information

The project uses the **Online Retail dataset**, which contains transactional data from an e-commerce retailer.

The dataset includes the following information:

- Invoice Number
- Stock Code
- Product Description
- Quantity
- Invoice Date
- Unit Price
- Customer ID
- Country

### Dataset Size

- **Original Records:** 541,909
- **Final Cleaned Records:** 397,884
- **Unique Customers Analyzed:** 4,338

---

## 🧹 Data Cleaning and Preprocessing

The following data cleaning steps were performed:

- Checked dataset structure and data types.
- Identified missing values.
- Removed records with missing `CustomerID`.
- Removed records with missing product descriptions.
- Identified and removed cancelled transactions.
- Removed transactions with zero or negative quantities.
- Removed transactions with zero or negative unit prices.

---

## 💰 Feature Engineering

A new feature called `TotalAmount` was created using:

```text
TotalAmount = Quantity × UnitPrice
````

This feature was used to calculate customer spending and support the RFM analysis.

---

## 📊 Customer Purchasing Behaviour Analysis

Customer-level metrics were calculated, including:

* **Purchase Frequency:** Number of unique invoices/orders associated with each customer.
* **Average Purchase Value:** Average transaction value based on purchase records.
* **Customer Lifetime Value:** Total amount spent by each customer during the available dataset period.

### Key Metrics

* **Average Purchase Value:** 68.35
* **Average Purchase Frequency:** 4.27
* **Average Customer Lifetime Value:** 2,054.27

---

# 👥 RFM Analysis

RFM analysis was used to understand customer purchasing behaviour.

### Recency

Number of days since a customer's most recent purchase.

### Frequency

Number of unique purchases made by a customer.

### Monetary

Total amount spent by a customer.

These three features were used as the primary inputs for customer segmentation.

---

## ⚙️ Feature Scaling

The RFM features were standardized using:

```python
StandardScaler()
```

Standardization ensures that Recency, Frequency, and Monetary values are placed on a comparable scale before applying the K-Means clustering algorithm.

---

## 🎯 K-Means Clustering

The **Elbow Method** was used to determine an appropriate number of clusters.

Based on the analysis, the customer base was segmented into:

```text
4 Customer Clusters
```

The clusters were then analyzed based on their average Recency, Frequency, and Monetary values.

---

## 🔍 Customer Segments

| Segment           | Customers | Avg. Recency | Avg. Frequency | Avg. Monetary |
| ----------------- | --------: | -----------: | -------------: | ------------: |
| Regular Customers |     3,054 |        43.70 |           3.68 |      1,359.05 |
| At-Risk Customers |     1,067 |       248.08 |           1.55 |        480.62 |
| VIP Customers     |        13 |         7.38 |          82.54 |    127,338.31 |
| Loyal Customers   |       204 |        15.50 |          22.33 |     12,709.09 |

### Segment Description

#### 🏆 VIP Customers

A small group of highly valuable customers with very recent purchases, extremely high purchase frequency, and the highest spending.

#### 🤝 Loyal Customers

Customers who purchase frequently, have purchased recently, and generate strong revenue.

#### 👥 Regular Customers

The largest customer segment with moderate purchasing frequency and spending behaviour.

#### ⚠️ At-Risk Customers

Customers with a high recency value, indicating that they have not made purchases recently and may require re-engagement.

---

## 📈 Visualizations Included

The project includes the following visualizations:

* Elbow Method for Optimal Number of Clusters
* Number of Customers by Cluster
* Recency vs Frequency Customer Segmentation
* Frequency vs Monetary Customer Segmentation
* Average Customer Spending by Segment

---

## 💡 Marketing Recommendations

### 🏆 VIP Customers

* Provide exclusive rewards and premium loyalty benefits.
* Offer personalized recommendations.
* Provide early access to new products.
* Focus on retention through personalized customer experiences.

### 🤝 Loyal Customers

* Introduce loyalty programs and reward points.
* Encourage higher spending through cross-selling and upselling.
* Provide personalized product recommendations.

### 👥 Regular Customers

* Use targeted promotions to encourage more frequent purchases.
* Recommend related products based on purchasing behaviour.
* Offer incentives to increase engagement and spending.

### ⚠️ At-Risk Customers

* Launch re-engagement campaigns.
* Offer personalized discounts or limited-time promotions.
* Use targeted communication to encourage customers to return.

---

## 📊 Key Insights

1. **Regular Customers represent the largest customer segment**, with 3,054 customers and moderate purchasing behaviour.

2. **At-Risk Customers account for 1,067 customers** and have the highest average recency of 248.08 days, indicating a significant period since their last purchase.

3. **VIP Customers represent a very small but highly valuable segment**, consisting of only 13 customers with the highest purchase frequency and spending.

4. **Loyal Customers demonstrate strong purchasing behaviour**, with an average purchase frequency of 22.33 and average monetary value of 12,709.09.

5. The analysis indicates that customer value is concentrated among a relatively small number of VIP and Loyal customers, highlighting the importance of customer retention strategies.

---

## 📌 Conclusion

This project used **RFM analysis and K-Means clustering** to segment 4,338 customers into four distinct groups based on their purchasing behaviour.

The analysis identified:

* 🏆 VIP Customers
* 🤝 Loyal Customers
* 👥 Regular Customers
* ⚠️ At-Risk Customers

The results show that while Regular Customers represent the largest group, VIP and Loyal Customers generate significantly higher value. At-Risk Customers represent an important opportunity for targeted re-engagement campaigns.

These insights can support better decision-making in areas such as **customer retention, personalized marketing, loyalty programs, cross-selling, upselling, and customer engagement**.

---

## 📁 Repository Structure

```text
Task_2_Customer_Segmentation/
│
├── Customer_Segmentation_Analysis.ipynb
├── Online Retail.xlsx
└── README.md
```

---

## 👨‍💻 Author

**Praveen Patil**
Data Analytics Intern | Oasis Infobyte

```
