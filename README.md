# 💳 Credit Card Fraud Detection

## 📌 Project Overview
This project focuses on detecting fraudulent credit card transactions using machine learning. The goal is to build a classification model that can distinguish between genuine and fraudulent transactions, helping financial institutions minimize losses and protect customer data.

---

## 📁 Dataset
- **Source**: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- **Description**:
  - Contains transactions made by European cardholders in September 2013.
  - **Total Records**: 284,807
  - **Fraudulent Transactions**: 492 (highly imbalanced)
  - Features are numerical and PCA-transformed for confidentiality, except `Time` and `Amount`.

---

## ⚙️ Technologies Used
- Python
- NumPy, Pandas
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🔍 Key Steps

### 1. Data Preprocessing
- Checked for null/missing values
- Handled class imbalance using **SMOTE (Synthetic Minority Over-sampling Technique)** or **undersampling**

### 2. Exploratory Data Analysis (EDA)
- Visualized class distribution
- Correlation heatmaps and amount/time-based fraud patterns

### 3. Feature Engineering
- Scaled `Amount` and `Time` using StandardScaler
- Dropped unnecessary features

### 4. Model Training
- Used classifiers like:
  - Logistic Regression
  - Random Forest
  - Decision Tree
  - XGBoost (optional)
- Performed cross-validation and grid search for tuning

### 5. Evaluation Metrics
- Confusion Matrix
- Precision, Recall, F1-Score
- ROC-AUC Curve

---

## 🎯 Results
- Models achieved **high precision and recall**, especially with balanced datasets
- Random Forest and XGBoost provided the best results for fraud detection
- ROC-AUC score: ~0.98 for top models

---

## ✅ Conclusion
The model effectively detects fraudulent transactions, even with severe class imbalance. Techniques like SMOTE and careful evaluation metrics ensure the model is reliable in real-world applications.
