# 🎗️ Breast Cancer Diagnostic Classification



## 📌 Project Overview
This project focuses on identifying whether a breast tumor is **Malignant (1)** or **Benign (0)** based on diagnostic features. The goal is to build a highly accurate predictive model to assist in medical decision-making using the Wisconsin Diagnostic Breast Cancer (WDBC) dataset.

---

## 📊 Dataset Information
- **Source:** UCI Machine Learning Repository / Kaggle.
- **Samples:** 569.
- **Features:** 30 clinical features (radius, texture, perimeter, area, smoothness, etc.).
- **Target Variable:** Diagnosis (M = Malignant, B = Benign).

---

## 🛠️ Project Workflow

### 1. Data Cleaning & Preparation
- Removed unnecessary columns (`id`, `Unnamed: 32`).
- Encoded categorical target variables into numerical values (M: 1, B: 0).

### 2. Exploratory Data Analysis (EDA)
- Generated visual comparisons between Malignant and Benign cases using **Boxplots**.
- Analyzed feature distributions and variances across classes.

### 3. Data Balancing & Scaling
- **SMOTE (Synthetic Minority Over-sampling Technique):** Applied to handle any potential class imbalance and ensure the model generalizes well.
- **MinMaxScaler:** Scaled features to a range of (0, 1) to improve the performance of the Logistic Regression model.

### 4. Modeling & Training
- Algorithm: **Logistic Regression**.
- Split: 80% Training, 20% Testing.
- Evaluation Metrics: Accuracy, Confusion Matrix, and Classification Report (Precision, Recall, F1-Score).

### 5. Model Persistence
- Saved the trained model (`model.pkl`) and the scaler (`scaler.pkl`) using **Joblib** for future deployment.

---

## 💻 Tech Stack
- **Data Manipulation:** `Pandas`, `NumPy`
- **Visualization:** `Seaborn`, `Matplotlib`
- **Machine Learning:** `Scikit-Learn`
- **Oversampling:** `Imbalanced-learn (SMOTE)`
- **Model Storage:** `Joblib`

---

## 📈 Results
- **Training Accuracy:** [97]%
- **Testing Accuracy:** [98]%
- The model shows strong performance in detecting Malignant cases with a high Recall rate, minimizing False Negatives in a medical context.

