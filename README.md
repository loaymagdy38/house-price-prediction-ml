# 🏠 House Price Prediction - Machine Learning Project

## 🚀 Project Overview
End-to-End Machine Learning pipeline for price prediction using Linear & Ridge Regression, covering full data preprocessing, feature engineering, model evaluation, and performance comparison.

This project demonstrates a complete regression workflow from raw data to final model selection.

---

## 🔄 Workflow

- Data Loading
- Exploratory Data Analysis (EDA)
- Data Cleaning
- Handling Missing Values
- Removing Duplicates
- Outlier Detection (IQR Method)
- Feature Engineering
- Encoding Categorical Variables
- Feature Scaling
- Model Training & Evaluation
- Model Comparison

---

## 📂 Dataset Information

- Total samples: **8128**
- Features: **12**
- Target variable: `selling_price`

### Main Features
- year
- km_driven
- fuel
- transmission
- engine
- max_power
- seats
- owner
- seller_type
- mileage

---

## 🔍 Data Preprocessing

### 1️⃣ Handling Missing Values
Missing values in:
- mileage
- engine
- max_power
- seats

Filled using **median imputation**.

---

### 2️⃣ Handling Duplicates
- Duplicated rows detected: **1202**
- After cleaning: **0 duplicates**

---

### 3️⃣ Handling Outliers
Outliers removed using the **IQR (Interquartile Range) method** for:
- selling_price
- km_driven
- mileage
- engine
- max_power
- seats
- year

---

### 4️⃣ Feature Engineering
- Extracted numeric values from `max_power`
- Applied **One-Hot Encoding** to categorical variables
- Applied **StandardScaler** to numeric features

---

## 🤖 Models Implemented

- Linear Regression
- Ridge Regression (α = 1.0)

---

## 📊 Model Evaluation

| Model | RMSE | R² Score |
|-------|------|----------|
| Linear Regression | 112,070 | 0.756 |
| Ridge Regression | 112,058 | 0.7564 |

🔎 Ridge Regression slightly outperforms Linear Regression.

---

## 📈 Visualizations

- Actual vs Predicted Plot
- Residuals vs Predicted Plot
- RMSE Comparison
- R² Comparison

---

## 🏆 Conclusion

Ridge Regression was selected as the best-performing model due to slightly better generalization and slightly lower RMSE.

The model explains approximately **75% of the variance** in house prices.

---

## 🛠 Tech Stack

Python • Pandas • NumPy • Matplotlib • Seaborn • Scikit-learn
