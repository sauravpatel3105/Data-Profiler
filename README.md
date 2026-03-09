Here is a **professional README.md file** for your **Customer Churn Data Profiler Project** based on your dataset, code, EDA graphs, and insights.

---

# Customer Churn Prediction – Data Profiler Project

## Project Overview

This project focuses on **data preprocessing, exploratory data analysis (EDA), feature engineering, and machine learning modeling** to predict **customer churn**. The goal is to analyze customer purchase behavior and identify factors that influence whether a customer will stop using a service or purchasing products.

The project integrates data from **multiple sources (CSV, JSON, SQL database, and API)**, performs cleaning and transformation, and builds machine learning models to predict churn.

A full automated profiling report was also generated using **YData Profiling**.
You can view it here:
**Customer Profiling Report:** 

---

# Problem Statement

Customer churn occurs when customers stop purchasing or using a company’s services. Predicting churn helps businesses take proactive actions such as:

* Personalized marketing
* Customer engagement programs
* Discounts and loyalty rewards

This project treats churn prediction as a **binary classification problem** (Churn = 0 or 1). 

---

# Dataset Description

The dataset contains **customer demographic, behavioral, and engagement data**.

Example features include:

| Feature                 | Description                           |
| ----------------------- | ------------------------------------- |
| Age                     | Age of the customer                   |
| Gender                  | Customer gender                       |
| City                    | Customer location                     |
| Income                  | Annual income                         |
| Purchase_Frequency      | Number of purchases                   |
| Total_Spending          | Total spending amount                 |
| Last_Purchase_Days_Ago  | Days since last purchase              |
| Preferred_Channel       | Purchase channel (Store, App, Online) |
| Customer_Tenure_Years   | Relationship duration                 |
| Support_Calls_Last_Year | Number of complaints                  |
| Discount_Usage_Rate     | Discount usage percentage             |
| Engagement_Score        | Customer engagement level             |
| Churn                   | Target variable (0 = No, 1 = Yes)     |

Sample data structure is shown in the API dataset file. 

---

# Project Workflow

## 1 Data Acquisition

Data was collected from multiple sources:

* CSV file
* JSON file
* SQL database
* API JSON data

All datasets were merged into a single dataframe for analysis. 

---

# 2 Data Cleaning

The following preprocessing steps were performed:

* Removed duplicate records
* Handled missing values
* Converted data types
* Encoded categorical variables
* Dropped unnecessary columns

Numerical missing values were filled using **mean imputation**, and categorical values using **mode imputation**. 

---

# 3 Exploratory Data Analysis (EDA)

EDA was performed to understand customer behavior.

### Age Distribution

Most customers fall between **25–55 years old**, showing a balanced age distribution.

### Income Distribution

Customer income ranges from **30,000 to 200,000**, indicating diverse purchasing power.

### Churn Distribution

The dataset shows **class imbalance**, where non-churn customers are higher than churn customers.

### Gender vs Churn

Gender has **minimal impact** on churn behavior.

### Correlation Analysis

Important churn indicators include:

* Last Purchase Days Ago
* Engagement Score
* Purchase Frequency
* Support Calls

Behavioral metrics influence churn more than demographic factors. 

---

# Feature Engineering

A new feature was created:

**Avg_Spending**

```
Avg_Spending = Total_Spending / Purchase_Frequency
```

This helps measure **customer value per transaction** and improves model performance. 

---

# Machine Learning Models

Two machine learning models were implemented:

### 1 Logistic Regression

* Used as a baseline model
* Simple and interpretable

### 2 Random Forest

* Captures complex patterns
* Handles nonlinear relationships
* Provided better predictive performance

The model evaluation includes:

* Accuracy Score
* Confusion Matrix
* Classification Report

The output report shows model accuracy and performance metrics. 

---

# Feature Importance

Top features influencing churn:

1. Last_Purchase_Days_Ago
2. Engagement_Score
3. Support_Calls_Last_Year
4. Purchase_Frequency
5. Income

These variables significantly impact churn prediction.

---

# Key Insights

Important findings from the analysis:

* Customers inactive for **180+ days** are more likely to churn.
* Low engagement score strongly indicates churn risk.
* Customers with **frequent support complaints** have higher churn probability.
* Purchase behavior influences churn more than demographic attributes.

---

# Business Recommendations

Based on insights, companies should:

* Target inactive customers with personalized offers
* Improve engagement through loyalty programs
* Monitor customers with high support calls
* Reward high-spending customers

These strategies can reduce churn and improve retention. 

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* SQLite
* YData Profiling

Dependencies are listed in the requirements file. 

---

# Project Structure

```
Customer-Churn-Data-Profiler
│
├── customers_churn_dataset.csv
├── customers_churn_dataset.json
├── customers_churn_database.db
├── customers_churn_api_sample.json
│
├── data_profiler.py
├── requirements.txt
│
├── Python Output.pdf
├── PROJECT INSIGHT.pdf
├── Part_A_Fundamentals.pdf
│
└── Customer_Churn_Profile_Report.html
```

---

# Conclusion

The **Customer Churn Data Profiler project** demonstrates the full data science workflow including **data integration, cleaning, exploratory analysis, feature engineering, and machine learning modeling**.

The analysis shows that **customer behavior metrics such as engagement, inactivity, and support interactions are the strongest predictors of churn**, enabling businesses to take proactive retention strategies.

---

If you want, I can also give you a **GitHub-ready README (with badges + project screenshots + better formatting)** that looks **much more professional for recruiters.**
