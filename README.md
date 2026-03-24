# 🚀 Task 2: End-to-End ML Pipeline for Customer Churn Prediction

## 📌 Project Overview
Customer churn prediction is a critical business challenge. In this project, I built a **reusable and production-ready machine learning pipeline** using the **Scikit-learn Pipeline API**. The goal is to predict whether a customer is likely to leave the service based on their usage behavior and demographics.

---

## 🎯 Objectives
* **Build a unified pipeline** for automated data preprocessing and model training.
* **Implement scaling** (`StandardScaler`) and **categorical encoding** (`OneHotEncoder`).
* **Train and compare** high-performance models: **Logistic Regression** and **Random Forest**.
* **Optimize performance** using `GridSearchCV` for hyperparameter tuning.
* **Model Deployment:** Export the final model using `joblib` for real-world use.

---

## 🛠️ Methodology & Approach

### 1. Data Loading & Cleaning
* **Source:** Telco Customer Churn dataset.
* **Cleaning:** Handled missing values in `TotalCharges` and converted the column to numeric format.
* **Feature Selection:** Dropped unnecessary IDs and mapped the target variable (`Churn`) to numerical values (1/0).

### 2. Exploratory Data Analysis (EDA)
* **Churn Distribution:** Visualized the balance between staying and churning customers.
* **Correlation Heatmap:** Identified that **Tenure** has a strong negative correlation with Churn (loyal customers stay longer).
* **Monthly Charges:** Observed that customers with higher monthly costs are more likely to churn.

### 3. Automated ML Pipeline
* Created a `ColumnTransformer` to handle different data types automatically.
* Integrated the preprocessing steps and the classifier into a single `Pipeline` object to prevent data leakage and ensure consistency.

---

## 📊 Evaluation & Key Results
* **Final Accuracy Score:** ~82%
* **Best Model:** Found via `GridSearchCV` (Logistic Regression/Random Forest).
* **Confusion Matrix Insights:** * **True Negatives (939):** High accuracy in identifying loyal customers.
    * **True Positives (222):** Successfully caught 222 potential churners for proactive retention.

---

## 📂 Deliverables
* `Customer_Churn_Pipeline.ipynb`: Full documented code and visualizations.
* `churn_pipeline_model.pkl`: The exported, ready-to-use pipeline model.
* `README.md`: This project documentation.

---
##👤 Author & Organization

Author: Hatem Ali

Student ID: DHC-1079

Organization: DevelopersHub Corporation

**Date:** March 2026

