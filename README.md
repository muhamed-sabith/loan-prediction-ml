# 🏦 Loan Approval Prediction Using Machine Learning

## 📌 Project Overview
This project builds a Machine Learning model to predict whether a loan application will be approved or rejected based on applicant details such as income, credit history, loan amount, and property area.

The goal is to help financial institutions automate loan approval decisions using data-driven insights.

---

## 📊 Dataset Information
- Total Records: 614 loan applications
- Features: Applicant income, co-applicant income, credit history, loan amount, education, property area, etc.
- Target Variable: `Loan_Status`
  - 1 → Approved
  - 0 → Not Approved

---

## ⚙️ Project Workflow

### 1️⃣ Data Preprocessing
- Removed unnecessary columns (`Loan_ID`)
- Handled missing values:
  - Mode for categorical features
  - Median for numerical features
- Converted categorical variables using One-Hot Encoding
- Scaled features using StandardScaler

### 2️⃣ Train-Test Split
- 80% Training Data
- 20% Testing Data
- Used `random_state=42` for reproducibility

### 3️⃣ Model Building
Two classification models were implemented and compared:

- Logistic Regression
- Random Forest Classifier

### 4️⃣ Model Evaluation
Evaluation metrics used:
- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)

---

## 📈 Results

| Model                  | Accuracy |
|------------------------|----------|
| Logistic Regression    | 78.86%   |
| Random Forest          | ~78%     |

Logistic Regression slightly outperformed Random Forest and was selected as the final model due to similar performance and better interpretability.

---

## 📊 Confusion Matrix Insights
- Strong performance in predicting approved loans
- Some false positives (risk approval cases)
- Very low false negatives

This indicates the model is effective but can be improved for risk-sensitive environments like banking.

---

## 🛠 Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook (VS Code)

---

## 🚀 Future Improvements
- Hyperparameter tuning (GridSearchCV)
- Feature importance analysis
- Cross-validation
- Model deployment using Streamlit or Flask
- ROC-AUC analysis

---

## 📂 Project Structure

```
loan-prediction-ml/
│
├── data/          # Dataset files
├── notebook/      # Jupyter notebook (analysis & modeling)
├── model/         # Saved trained models (future use)
└── README.md
```

---

## 🎯 Conclusion
This project demonstrates an end-to-end Machine Learning workflow:
- Data Cleaning
- Feature Engineering
- Model Training
- Model Evaluation
- Model Comparison

It reflects practical implementation skills required for entry-level Data Science and Data Analyst roles.

---