The [Promotional Campaign Analysis Notebook](https://colab.research.google.com/drive/1_GWTTxz0igCZF84CNCO1cDzjZNwIUeih#scrollTo=3e453293-5efd-4ad8-afd5-cd8ea61f31db) implements a machine learning model to predict customer response to a discount campaign for a retail store.

# Introduction

The retail store is launching a 40% discount offer and aims to target customers most likely to accept it. By developing a machine learning model, we can predict customer behavior and optimize the outreach strategy.

## Problem Statement

The offer will be extended to existing customers via phone calls. The marketing team seeks to identify the probability of a customer accepting the offer and the key factors influencing their decision.

## Data

The dataset consists of historical consumer transaction information and their response to a previous discount offer.

Target Variable: Response (1: Accepted offer, 0: Rejected offer)
Numeric Variables:
- Age (calculated from Year_Birth)
- Years of Patronage (calculated from Dt_Customer)
- Income
- Spending on various product categories (fish, meat, fruits, etc.)
- Number of purchases made through different channels (web, store, catalog)
- Number of website visits in the last month
- Recency (number of days since the last purchase)

Categorical Variables:
- Education level
- Marital status

Source: https://www.kaggle.com/datasets

# Code Structure

- Import Libraries: pandas, numpy, seaborn, matplotlib, etc.
- Data Loading: Read the CSV file using pandas.

Exploratory Data Analysis (EDA):
- Check data shape, data types, missing values, duplicates.
- Analyze distribution of categorical variables.
- Calculate descriptive statistics for numerical variables.
- Calculate correlation coefficients between independent and dependent variables.
- Visualize relationships between variables using histograms and scatter plots.

Data Preprocessing:
- Handle missing values in the Income field (e.g., imputation).
- Replace irrelevant categories in Marital Status with a more appropriate label.
- Create new features (Age, Years of Patronage)
- Encode categorical variables using one-hot encoding.
- Split data into features (X) and target variable (y).
- Split data into training and testing sets.

Modeling:
- Train and evaluate different machine learning models (e.g., Logistic Regression, Random Forest, SVM).
- Evaluate model performance using metrics like accuracy, precision, recall, F1-score, and confusion matrix.

Prediction:
- Demonstrate model prediction on a sample customer record.

Conclusion:
- Key findings from the analysis.
