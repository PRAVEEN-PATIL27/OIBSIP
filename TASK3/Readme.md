# 🧹 Employee Data Cleaning and Preprocessing

## 📝 Project Overview

This project was completed as part of the **Oasis Infobyte Data Analytics Internship – Task 3**.

The project focuses on cleaning and preprocessing a messy employee dataset to improve its quality, consistency, and usability for further analysis.

The dataset was examined to identify data quality issues such as missing values, incorrect data types, invalid phone number formatting, duplicate records, and potential outliers. Appropriate data cleaning techniques were applied, followed by final validation to ensure that the dataset is clean and analysis-ready.

---

## 🎯 Project Objectives

The main objectives of this project are to:

- Inspect the employee dataset and understand its structure.
- Identify missing values and data quality issues.
- Handle missing values using appropriate statistical methods.
- Check for duplicate records.
- Correct inconsistent data types and formatting issues.
- Detect potential outliers using the IQR method.
- Validate the cleaned dataset.
- Export a clean and analysis-ready dataset.

---

## 🛠️ Technologies Used

- Python
- Google Colab
- Pandas
- NumPy

---

## 📂 Dataset Information

The original dataset contains employee-related information with:

- **1,020 Records**
- **12 Columns**

### Columns Included

- Employee_ID
- First_Name
- Last_Name
- Age
- Department_Region
- Status
- Join_Date
- Salary
- Email
- Phone
- Performance_Score
- Remote_Work

---

## 🔍 Data Quality Issues Identified

The initial data quality assessment identified the following issues:

| Issue | Result |
|---|---:|
| Missing Values in Age | 211 |
| Missing Values in Salary | 24 |
| Total Missing Values | 235 |
| Duplicate Rows | 0 |
| Negative Phone Numbers | 1,020 |
| Join_Date Data Type | Object |

---

## 🧹 Data Cleaning Performed

### 1. Missing Value Treatment

Missing values were identified in the following columns:

- **Age:** 211 missing values
- **Salary:** 24 missing values

Both columns were cleaned using **median imputation**.

After cleaning:

- **Remaining Missing Values: 0**

---

### 2. Duplicate Record Check

The dataset was checked for duplicate rows.

- **Duplicate Rows Found: 0**

Therefore, no records needed to be removed.

---

### 3. Data Type Conversion

The `Join_Date` column was originally stored as an `object` data type.

It was converted to:

```text
datetime64[ns]
````

This makes the date column suitable for further date-based analysis.

---

### 4. Phone Number Cleaning

The `Phone` column contained negative values because it was stored as a numeric data type.

The following cleaning steps were performed:

* Converted the column to text format.
* Removed negative signs.
* Preserved phone numbers as identifiers rather than numerical values.

After cleaning:

* **Phone numbers with negative signs: 0**

---

### 5. Outlier Detection

Outlier detection was performed on:

* Age
* Salary

The **Interquartile Range (IQR) method** was used.

### Results

| Column | Outliers Detected |
| ------ | ----------------: |
| Age    |                 0 |
| Salary |                 0 |

Since no outliers were detected, no records were removed or modified.

---

## 📊 Before vs After Cleaning Summary

| Metric                 | Before Cleaning | After Cleaning |
| ---------------------- | --------------: | -------------: |
| Total Rows             |           1,020 |          1,020 |
| Total Columns          |              12 |             12 |
| Missing Values         |             235 |              0 |
| Duplicate Rows         |               0 |              0 |
| Negative Phone Numbers |           1,020 |              0 |
| Age Outliers           |               0 |              0 |
| Salary Outliers        |               0 |              0 |
| Join_Date Data Type    |          object | datetime64[ns] |

---

## 💡 Key Findings

* The dataset originally contained **1,020 employee records** and **12 columns**.
* A total of **235 missing values** were identified.
* Missing values in `Age` and `Salary` were successfully handled using median imputation.
* No duplicate records were found.
* All **1,020 phone numbers** had negative signs removed.
* `Join_Date` was successfully converted from `object` to `datetime64[ns]`.
* No outliers were detected in the `Age` and `Salary` columns using the IQR method.
* All **1,020 original records** were retained.
* The final dataset contains **0 missing values**.

---

## 📁 Repository Structure

```text
Task_3_Data_Cleaning/
│
├── After_cleaning_analysis.csv
├── Before_cleaning_analysis.csv
├── OIBSIP_Task3_Data_Cleaning.ipynb
└── Readme.md
```

---

## 📌 Conclusion

This project successfully transformed a messy employee dataset into a clean, structured, and analysis-ready dataset.

The data cleaning process addressed missing values, incorrect data types, and invalid phone number formatting. The dataset was also checked for duplicate records and potential outliers.

Final validation confirmed that the dataset contains **0 missing values**, corrected data formats, and no remaining negative phone number formatting issues.

The cleaned dataset was exported as:

```text
Cleaned_Employee_Dataset.csv
```

The final dataset can now be used for further **data analysis, visualization, and machine learning applications**.

---

## 👨‍💻 Author

**Praveen Patil**

Data Analytics Intern – Oasis Infobyte

````
