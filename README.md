# 🩺 Predicting Diabetes with Logistic Regression – A Healthcare ML Project

Welcome! This is a mini-project where I explored building a machine learning model to **predict diabetes** using the [Pima Indians Diabetes dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database).  
It helped me gain hands-on experience with the **ML pipeline in healthcare** and overcome my fear of **statistical visualizations** step by step. 😊

---

## 📌 Project Goals

- Clean and explore real-world healthcare data
- Build and evaluate a Logistic Regression classifier
- Improve it using **hyperparameter tuning**
- Learn to interpret model outputs like **ROC AUC**, **feature importance**, and **confusion matrices**

---

## 📊 Dataset Overview

- 768 rows, 9 columns
- Features include: Glucose, BMI, Age, Blood Pressure, etc.
- Target variable: `Outcome` (1 = Diabetes, 0 = No Diabetes)

---

## ✅ ML Pipeline Overview

### 1. Data Cleaning

- Replaced **invalid values** (e.g., 0 for Blood Pressure) with `NaN`
- Imputed missing values using **column mean**

### 2. Visual Exploration

- Used **Seaborn heatmaps** to understand correlations
- Analyzed feature distributions using histograms

### 3. Feature Scaling

- Applied **StandardScaler** to normalize input features

### 4. Initial Modeling

- Trained a **Logistic Regression** model
- ROC AUC on test set: ~0.82

### 5. Model Tuning

- Used **GridSearchCV** with cross-validation to find best parameters:

```python
{'C': 10, 'penalty': 'l1', 'solver': 'liblinear'}
```
- Cross-validated ROC AUC: ~0.84

### 6. Final Evaluation

- ROC AUC on test set: 0.84
- Confusion Matrix and Classification Report showed balanced performance
- Interpreted L1 feature importance to see which health factors mattered most (like Glucose and BMI)

## 🔍 What I Learned

- How to build a real ML pipeline
- Importance of data visualization for insight and debugging
- How cross-validation prevents overfitting
- How to interpret ROC AUC and model coefficients in a healthcare context
- Impact of hyperparameter tuning
- That I can actually enjoy and get over my fear of statistics 😄
