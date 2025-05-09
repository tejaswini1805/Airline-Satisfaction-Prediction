# ✈️ Predicting Airline Passenger Satisfaction  
*A Machine Learning Approach to Improve Service Quality*

---

## 🔒 Problem Statement

This project analyzes **airline passenger satisfaction survey data** to predict satisfaction levels based on various demographic, flight-related, and service factors.  
The goal is to identify key drivers of passenger satisfaction and build a reliable predictive model to help airlines enhance their services.

---

## 🎯 Objectives

- Analyze factors influencing passenger satisfaction and dissatisfaction.
- Build and evaluate machine learning models to predict satisfaction levels.
- Select the best-performing model for deployment and actionable insights.

---

## 📊 Dataset Overview

- **Data Source:** Passenger satisfaction survey results
- **Features Include:**
  - Demographics (Age, Gender)
  - Flight details (Class, Distance)
  - Onboard services (Food, Entertainment, Cleanliness)
  - Airport and check-in services

---

## 🚀 Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Analyzed satisfaction patterns across demographics and services.
- Visualized correlations and feature distributions.
- Identified key pain points impacting passenger experience.

### 2. Data Preprocessing
- Handled missing values and outliers.
- Encoded categorical variables.
- Normalized numerical features for model performance.

### 3. Model Building & Evaluation
Tested multiple models:
- Logistic Regression ❌ (Overfitting & low generalization)
- Random Forest & Decision Tree ❌ (Overfitting with 100% training accuracy)
- Gradient Boosting ✅ (Good generalization)
- **XGBoost** ✅ (Best performer)

### 4. Model Selection: XGBoost
Based on **k-fold Cross-Validation**:
- Mean ROC AUC (XGBoost): **0.9951**
- Mean ROC AUC (Gradient Boosting): 0.9944
- XGBoost showed:
  - Higher accuracy
  - Better stability (lower standard deviation)
  - Stronger generalization
  - Regularization to control overfitting

---

## ✅ Final Model Evaluation (XGBoost)

### 🔎 Confusion Matrix
- True Negatives (0): 42,321  
- False Positives (1): 2,576  
- False Negatives (0): 997  
- True Positives (1): 57,700  

### 📊 Classification Report
| Metric      | Class 0 (Dissatisfied) | Class 1 (Satisfied) |
|-------------|-----------------------|--------------------|
| Precision   | 0.98                  | 0.96              |
| Recall      | 0.94                  | 0.98              |
| F1-Score    | 0.96                  | 0.97              |

- **Overall Accuracy:** 97%

### 📈 Analysis
- High accuracy and balanced precision-recall.
- Model identifies **98% of actual satisfied passengers** correctly.
- Good balance between **false positives and false negatives**.

---

## 🛠 Tech Stack

- **Python 3.7+**
- **Libraries:**
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `xgboost`
  - `matplotlib`
  - `seaborn`
  - `pickle`

---

## 💡 Key Conclusions
- **XGBoost** outperformed all other models in accuracy and stability.
- Achieved **97% overall accuracy** with strong generalization.
- Airlines can leverage these insights to enhance service quality and passenger experience.

---

## 📈 Potential Impact
- Identify the **biggest drivers** of passenger satisfaction and dissatisfaction.
- Help airlines improve:
  - In-flight services (food, entertainment)
  - Ground services (check-in, cleanliness)
  - Overall customer experience
- Enhance passenger loyalty and brand reputation.

---

⭐ **If you find this project helpful, feel free to star this repository!**  
