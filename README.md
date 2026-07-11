# Credit Risk Prediction using Logistic Regression and Random Forest

Machine Learning project for predicting **credit default risk** using the **UCI Default of Credit Card Clients** dataset. The project compares two supervised classification models—**Logistic Regression** and **Random Forest**—to identify customers with a high probability of defaulting on their credit card payments.

---

## Project Overview

Financial institutions use credit risk models to estimate the probability that a customer will fail to repay a loan or credit obligation. Accurate predictions help reduce financial losses while improving lending decisions.

This project includes:

- Exploratory Data Analysis (EDA)
- Data preprocessing
- Feature engineering
- Logistic Regression model
- Random Forest model
- Model evaluation using multiple classification metrics
- Confusion matrices
- ROC curves and AUC comparison

---

## Dataset

**Dataset:** UCI Default of Credit Card Clients

- Source: https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients
- File used: `UCI_Credit_Card.xls`

The dataset contains demographic information, payment history, bill statements, and previous payment records of Taiwanese credit card clients.

**Target variable**

- **target**
  - 0 → No Default
  - 1 → Default

---

## Technologies

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## Project Workflow

### 1. Data Loading

- Import dataset
- Verify dimensions
- Inspect data types
- Check missing values

---

### 2. Exploratory Data Analysis

Performed:

- Descriptive statistics
- Class distribution
- Correlation matrix
- Correlation with the target variable

---

### 3. Data Preprocessing

The preprocessing pipeline includes:

- Removing the ID column
- One-hot encoding categorical variables
- Train/Test split
- Feature standardization (Logistic Regression)

---

### 4. Machine Learning Models

### Logistic Regression

A linear probabilistic classifier commonly used in credit scoring because of its interpretability.

Configuration:

- solver = liblinear
- class_weight = balanced
- max_iter = 1000

---

### Random Forest

An ensemble learning algorithm based on multiple decision trees.

Configuration includes:

- 300 decision trees
- Bootstrap sampling
- Balanced class weights

---

## Model Evaluation

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix
- ROC Curve

---

## Results

The notebook compares both models using confusion matrices and ROC curves.

General observations:

- **Logistic Regression** achieves higher recall for the Default class, making it more suitable when identifying risky customers is the priority.
- **Random Forest** provides a better balance between precision and overall accuracy.
- The ROC-AUC metric is used to compare the discrimination capability of both models.


## References

Dataset:
https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients

---
