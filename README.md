# Customer Churn Prediction & Business Insights

## Overview

Customer churn is an important business problem because losing existing customers can directly affect revenue and customer lifetime value.

This project analyzes customer data from the IBM Telco Customer Churn dataset to identify patterns associated with churn and develop machine learning models for predicting customers who may be at risk of leaving.

The project covers the complete data science workflow, including data cleaning, exploratory data analysis, feature preprocessing, machine learning, model evaluation, and business insights.

## Project Objectives

- Explore customer behavior and churn patterns
- Clean and prepare customer data for analysis
- Identify factors associated with customer churn
- Build machine learning models to predict churn
- Compare models using appropriate evaluation metrics
- Translate analytical findings into useful business insights

## Dataset

The project uses the **IBM Telco Customer Churn dataset**, containing information about 7,043 customers.

The dataset includes:

- Customer demographics
- Account and contract information
- Internet and phone services
- Payment methods
- Monthly and total charges
- Customer tenure
- Churn status

The target variable for predictive modeling is **Churn Value**, where:

- `0` = Customer did not churn
- `1` = Customer churned

## Exploratory Data Analysis

The exploratory analysis identified several notable patterns in the dataset:

- Approximately **26.5%** of customers churned.
- Month-to-month customers showed higher churn than customers with longer contracts.
- Customers who churned generally had shorter tenure.
- Churned customers tended to have higher monthly charges.
- Fiber optic customers showed higher churn than DSL customers.
- Electronic check users showed the highest churn among payment methods.
- Customers without technical support showed considerably higher churn.

These findings represent associations in the available data and do not necessarily imply causal relationships.

## Data Cleaning

Several data quality checks and preprocessing steps were performed:

- Checked for duplicate customer records
- Examined missing values
- Converted `Total Charges` from text to numeric format
- Handled blank `Total Charges` values for customers with zero tenure
- Reviewed categorical and numerical features
- Identified variables that could introduce target leakage

## Machine Learning

The predictive modeling stage will compare multiple classification algorithms, including:

- Logistic Regression
- Random Forest
- XGBoost

Because the dataset contains more non-churned than churned customers, model performance will be evaluated using multiple metrics rather than accuracy alone:

- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

> **Status:** Exploratory data analysis is complete. Machine learning model development is currently in progress.
> ## Technologies

- **Programming:** Python
- **Data Analysis:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn, XGBoost
- **Development:** Jupyter Notebook
- **Dashboard:** Streamlit, Plotly
- **Version Control:** Git, GitHub

## Project Structure

```text
customer-churn-data-science-project/
│
├── data/
│   └── Telco_customer_churn.xlsx
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   └── 02_model_training.ipynb
│
├── src/
├── models/
├── dashboard/
├── requirements.txt
└── README.md
