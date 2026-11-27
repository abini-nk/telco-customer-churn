# 📊 Telco Customer Churn Prediction & Risk Analytics

<img width="1059" height="470" alt="download (1)" src="https://github.com/user-attachments/assets/011e7ebf-9123-4ef7-ba24-3ca226e3653c" />

## 📌 Project Overview
An end-to-end customer churn prediction, SQL revenue risk analysis, Excel summarization, and interactive dashboarding pipeline built on the IBM Telco Customer Churn dataset to identify high-risk accounts early and support proactive retention strategies.

- **Dataset:** IBM Telco Customer Churn Dataset
- **Target Variable:** `Churn` (`Yes` / `No`)
- **Pipeline:** Data Cleaning → Encoding & Scaling → Class Imbalance Handling (`SMOTE`) → Model Evaluation → Risk Scoring & CSV Export → SQLite Analytics (`JOIN`, `GROUP BY`, `CTE`, `DENSE_RANK()`) → Excel Summary & Data Studio Dashboard

## 📈 Interactive Dashboard
- **Dashboard Link:** [Telco Customer Churn Risk Dashboard](https://datastudio.google.com/reporting/617bf2e6-9f09-4317-8574-1e8671941576/page/l8VEG)
- **High-Risk Summary:** **370** high-risk customers identified with **$23,771.56** in expected monthly revenue at risk, concentrated heavily in **Month-to-month** contracts, **Fiber optic** internet service, and **Electronic check** payments.

## 🛠️ Tech Stack & Tools
- **Language & Environment:** Python 3.x, Google Colab / Jupyter Notebook
- **Data & ML:** Pandas, NumPy, Scikit-Learn, Imbalanced-Learn (`SMOTE`), XGBoost
- **Database:** SQLite (`sqlite3`)
- **Visualization & BI:** Matplotlib, Seaborn, Microsoft Excel, Google Data Studio / Looker Studio

## 🚀 Model Performance Comparison

| Model | Key Metrics & Highlights |
| :--- | :--- |
| **Logistic Regression** | **ROC-AUC: 0.8403**, Churn Recall: **80%**, Accuracy: **74%** — strong early churn risk detection |
| **Random Forest** | **ROC-AUC: 0.8236**, Accuracy: **77%** — captures non-linear feature interactions |
| **XGBoost** | **ROC-AUC: 0.8192**, Accuracy: **78%** — balanced overall classification performance |

## 💡 Key Business Insights & Recommendations
1. **Early Tenure & Month-to-Month Risk:** Month-to-month customers in the **0–12m** tenure group show high churn exposure (**52.50%** churn rate in grouped analysis); prioritize early onboarding and retention outreach.
2. **Contract & Payment Friction:** Risk clusters around **Month-to-month** contracts, **Fiber optic** users, and **Electronic check** payments; offer contract upgrade incentives and auto-pay adoption.
3. **Prioritized Retention:** Rank high-risk customers by expected monthly revenue at risk and `DENSE_RANK()` within contract segments to focus retention budgets where impact is highest.
