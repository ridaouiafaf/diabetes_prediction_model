# 🩺 Diabetes Prediction Using Logistic Regression

This is a simple machine learning project in which I used Logistic Regression to predict the likelihood of diabetes in patients using the Pima Indian Diabetes Dataset.

The primary goal of this project was to understand the full ML pipeline — from cleaning messy data and handling unusual values, to visualizing data relationships and interpreting model metrics like ROC AUC and confusion matrices.

---

## 💡 Motivation

I've always been intimidated by statistical visualizations — heatmaps, ROC curves, precision-recall... they felt abstract and overwhelming. This project is part of my learning journey to **face those fears** and deeply understand each concept by applying it project-by-project, especially in the context of **healthcare AI**.

---

## 📊 Dataset

- **Source**: [Pima Indians Diabetes Database on Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- **Features**: Includes patient metrics like glucose level, blood pressure, BMI, and age.
- **Target**: `Outcome` (1 = Diabetes, 0 = No Diabetes)

---

## ⚙️ Project Structure

├── data/ │ └── diabetes.csv ├── notebooks/ │ └── diabetes_prediction.ipynb ├── README.md └── requirements.txt


---

## 🔍 What I Did

- ✅ Handled unusual values (e.g., 0 blood pressure)
- ✅ Imputed missing values using column mean
- ✅ Visualized correlations using Seaborn heatmaps
- ✅ Preprocessed features with `StandardScaler`
- ✅ Split data into train/test
- ✅ Trained a **Logistic Regression** model
- ✅ Evaluated using:
  - Confusion Matrix
  - Classification Report
  - **ROC AUC Score: ~0.82**
  - **Cross-validation ROC AUC score: 5-Fold => [0.814, 0.800, 0.852, 0.886, 0.841] mean => 0.839**
---

## 📈 Key Results

- The model demonstrates strong predictive power, with a mean ROC AUC Score of 0.839 across 5-fold cross-validation — indicating consistent performance in distinguishing diabetic from non-diabetic cases.
- All ROC AUC scores across the folds were above 0.80, showing high stability and generalizability.
- Visualizations (like the correlation heatmap) highlighted that features such as glucose, BMI, and insulin have the strongest relationship with the diabetes outcome.

---

## 🧠 Learning Highlights

- Got comfortable using **Seaborn** for data visualization
- Understood how to **evaluate binary classification models**
- Learned the importance of **data preprocessing** (especially for health data!)
- Took one more step toward mastering ML in healthcare
