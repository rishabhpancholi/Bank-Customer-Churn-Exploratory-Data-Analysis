# Bank-Customer-Churn-Exploratory-Data-Analysis
Factors affecting churn of a bank's customers have been studied and inferences have been drawn using different kind of plots.

This project involves exploring and preprocessing a bank's customer dataset to analyze churn behavior (`Exited` column). It includes cleaning the data, performing exploratory data analysis (EDA), and preparing it for machine learning tasks.

---

## 📁 Dataset Overview

The dataset contains customer details from a bank, including demographics, account activity, and whether the customer exited the bank.

### 📌 Features:

- **CustomerId** – Unique identifier (to be dropped)
- **Surname** – Customer’s surname (to be dropped)
- **CreditScore** – Credit score of the customer
- **Geography** – Country of residence
- **Gender** – Gender of the customer
- **Age** – Age of the customer
- **Tenure** – Years with the bank
- **Balance** – Account balance
- **NumOfProducts** – Number of bank products used
- **HasCrCard** – Whether the customer has a credit card
- **IsActiveMember** – Whether the customer is active
- **EstimatedSalary** – Estimated annual salary
- **Exited** – Target variable (1 = exited, 0 = retained)

---

## 🛠️ Preprocessing Steps

### ✅ 1. Null Value Check
- Verified and handled missing values using `.isnull().sum()` and `.mean()`.

### 🔍 2. Unique Count per Column
- Used `.nunique()` to analyze feature uniqueness and spot potential identifiers.

### 🗑️ 3. Dropped Useless Columns
- Removed columns like `CustomerId` and `Surname` that do not contribute to the model.

### 🧾 4. Identified Column Types
- Categorized columns into **categorical** and **numerical** based on data type and value distribution.

---

## 📊 Exploratory Data Analysis (EDA)

### 📈 5. Target (`Exited`) vs Categorical Features
- Visualized the relationship between churn and:
  - **Geography**
  - **Gender**
  - **HasCrCard**
  - **IsActiveMember**

### 📉 6. Target (`Exited`) vs Numerical Features
- Plotted:
  - Age vs Exited
  - CreditScore vs Exited
  - Balance vs Exited
  - EstimatedSalary vs Exited

### 🔗 7. Correlation Matrix
- Generated a heatmap to study correlation between numeric features and the target variable.

---

## 🧰 Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

---
