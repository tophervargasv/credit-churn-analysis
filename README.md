# 🏦 Credit Card Churn Prediction

Predictive model to identify bank customers at risk of churning, 
using machine learning techniques applied to real financial data.

---

## 📌 Business Context

Customer churn is one of the most critical challenges for financial 
institutions. Losing a credit card customer means losing not only 
their direct revenue, but also cross-selling opportunities across 
other products.

This project analyzes a real dataset of 10,127 bank customers to:
- Identify behavioral patterns that predict churn
- Build a model that detects at-risk customers before they leave
- Translate data insights into actionable business recommendations

---

## 🔍 Key Findings

- **Transactional behavior** is the strongest churn predictor — 
  not demographics
- Customers with **fewer than 50 transactions** per period show 
  significantly higher churn risk
- Customers with **1-2 products** churn at 25-28% vs ~11% for 
  those with 4+ products
- Customers who **contacted the bank more** were more likely to 
  churn — suggesting unresolved issues drive cancellations

---

## 🤖 Models & Results

| Model | AUC-ROC | Accuracy | Recall (Churned) |
|---|---|---|---|
| Logistic Regression | 0.894 | 89% | 47% |
| **Random Forest** | **0.985** | **96%** | **81%** |

**Random Forest** was selected as the final model. It correctly 
identifies 81% of customers who will churn, with only 18 false 
alarms out of 1,701 active customers.

---

## 📁 Project Structure
credit-churn-analysis/
│
├── 01_exploracion_inicial.ipynb   # EDA & data cleaning
├── 02_modelo_predictivo.ipynb     # ML models & evaluation
├── BankChurners.csv               # Raw dataset (Kaggle)
├── data_limpia.csv                # Cleaned dataset
└── README.md                      # Project documentation

---

## 🛠️ Tech Stack

- **Python 3.11**
- pandas, numpy — data manipulation
- matplotlib, seaborn — visualization
- scikit-learn — machine learning

---

## 📊 Dataset

[Credit Card Customers — Kaggle](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers)

10,127 customers | 21 features | 16.1% churn rate

---

## 👤 Author

**Christopher Vargas**  
Economics & Finance  
[LinkedIn](https://linkedin.com/in/christophervvilla) | 
[GitHub](https://github.com/tophervargasv)