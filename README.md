# Fraud Detection Case Study

This project focuses on building a machine learning solution to proactively detect
fraudulent financial transactions using a large, highly imbalanced dataset.
The objective is not only to predict fraud accurately but also to derive actionable
business insights for fraud prevention.

---

## Business Problem
Financial institutions face significant losses due to fraudulent transactions.
The goal of this case study is to:
- Identify fraudulent transactions early
- Understand key drivers of fraud
- Propose practical prevention strategies based on model insights

---

## Dataset Overview
- Size: ~6.3 million transactions
- Target variable: `isFraud`
- Highly imbalanced dataset (fraud cases are rare)
- Mix of numerical and categorical features

---

## Approach
1. **Data Cleaning & Preprocessing**
   - Removed identifier columns with no predictive value
   - Handled skewed features using log transformation
   - Encoded categorical variables
   - Engineered balance-difference features
   - Checked multicollinearity using correlation analysis

2. **Modeling**
   - Logistic Regression (baseline model)
   - Random Forest (non-linear, stronger performance)
   - Addressed class imbalance using class weighting

3. **Evaluation**
   - Metrics used: Precision, Recall, F1-score, ROC-AUC
   - Recall prioritized due to high cost of missed fraud cases

4. **Interpretation & Insights**
   - Identified key fraud-driving features
   - Interpreted results using domain understanding

---

## Key Fraud Indicators
- Transaction type (TRANSFER, CASH_OUT)
- Large transaction amounts
- Sudden changes in account balances
- Abnormal destination account balance behavior

---

## Fraud Prevention Recommendations
- Real-time transaction risk scoring
- Multi-factor authentication for high-risk transactions
- Velocity and amount-based checks
- Continuous monitoring and periodic model retraining

---

## Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

---

## Files
- `Fraud_Detection_Case_Study.ipynb` – Complete analysis, modeling, and insights

---

## Outcome
This project demonstrates an end-to-end fraud detection workflow combining
machine learning techniques with business reasoning to support real-world
financial decision-making.
