# 📏 Height vs Weight Prediction using Linear Regression

## 📌 Project Overview
This project demonstrates how **Linear Regression** can be used to predict a person’s **weight (kg)** based on their **height (cm)**.  
The project covers the complete **data analysis and machine learning workflow**, including data exploration, outlier detection, preprocessing, model training, visualization, and evaluation.

---

## 📁 Dataset Description
- **Dataset Size:** 500 records  
- **Features:**
  - `Height_cm` → Height in centimeters (independent variable)
  - `Weight_kg` → Weight in kilograms (target variable)
- **Data Quality:** No missing values

> 📌 Note: Dataset is hosted externally due to size constraints.

---

## 🔍 Exploratory Data Analysis (EDA)
The following steps were performed to understand the data:

- Checked for missing values (none found)
- Visualized weight distribution using boxplots
- Scatter plot analysis between height and weight
- Identified relationship trends before modeling

---

## 🚨 Outlier Detection & Handling
Two statistical techniques were used:

### 🔹 1. Standard Deviation (3-Sigma Rule)
- Upper and lower bounds calculated using mean ± 3σ
- No extreme outliers detected using this method

### 🔹 2. Interquartile Range (IQR Method)
- Detected **4 outliers**
- Outliers were handled using **capping (winsorization)** instead of removal to preserve data size

---

## ⚙️ Data Preprocessing
- Selected `Height_cm` as feature (X)
- Selected `Weight_kg` as target (y)
- Train-test split:
  - **Training:** 80%
  - **Testing:** 20%

---

## 🤖 Machine Learning Model
- **Algorithm:** Linear Regression
- **Library Used:** scikit-learn
- **Why Linear Regression?**
  - Simple and interpretable
  - Ideal for continuous numerical prediction
  - Helps understand linear relationship between height and weight

---

## 📈 Model Visualization
- Scatter plot of height vs weight
- Best-fit regression line plotted over training data
- Clear positive linear relationship observed

---

## 📊 Model Evaluation
- **Evaluation Metric:** R² Score
- **R² Score:** **0.75**

This indicates that approximately **75% of the variance in weight** is explained by height.

---

## 🔢 Sample Prediction
Predicted weight for a person with **170 cm height**:
```text
≈ 53.15 kg
