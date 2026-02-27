# 🏦 Loan Approval Prediction – End-to-End ML Pipeline

## 📌 Project Overview
This project builds a complete Machine Learning pipeline to predict whether a loan application will be approved or rejected based on applicant information.

The workflow includes data preprocessing, model training, hyperparameter tuning, evaluation, explainability using SHAP, and model deployment readiness.

---

## 🎯 Objective
Predict `Loan_Status` (Approved = 1, Rejected = 0) using applicant features such as income, credit history, education, and property area.

---

## 📊 Dataset Information

- Total Samples: 614
- Features: 13
- Target Variable: `Loan_Status`
- Class Distribution:
  - Approved (Y): 422
  - Rejected (N): 192

The dataset contains both categorical and numerical features with missing values handled using imputation inside a preprocessing pipeline.

---

## ⚙️ Machine Learning Pipeline

The project uses a **Scikit-learn Pipeline** to ensure clean and production-ready modeling.

### Preprocessing:
- Missing value imputation
- Standard scaling (numerical features)
- One-hot encoding (categorical features)

### Model:
- Logistic Regression

### Hyperparameter Tuning:
- GridSearchCV (5-fold cross-validation)
- Optimized using F1-score

---

## 📈 Model Performance

Evaluation Metrics:
- Accuracy
- Confusion Matrix
- Classification Report
- ROC-AUC Score

The model was optimized for balanced performance using F1-score.

---

## 🔍 Model Explainability (SHAP)

SHAP (SHapley Additive exPlanations) was used to interpret model predictions.

The SHAP summary plot highlights the most influential features affecting loan approval decisions.

This ensures transparency and interpretability of predictions.

---

## 💾 Model Saving

The final trained pipeline (including preprocessing + model) is saved as:

---

## 🚀 How to Run This Project

1. Clone the repository:

2. Navigate to the project folder:

3. Install required dependencies:

4. Open and run the notebook:

Make sure `loan_data.csv` is present in the same folder before running the notebook.
