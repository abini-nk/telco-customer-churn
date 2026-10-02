# 📊 Telco Customer Churn Prediction

An end-to-end Machine Learning pipeline built in Python to predict customer churn for a telecommunications company. This project identifies high-risk churn customers and analyzes key behavioral features to support proactive customer retention strategies.

---

## 📌 Project Overview
Customer churn is a critical metric for subscription-based businesses. Predicting churn allows companies to intervene early with targeted retention offers.

This project covers:
- **Data Preprocessing & Cleaning:** Handled missing/coerce values in `TotalCharges` and performed One-Hot Encoding for categorical variables.
- **Class Imbalance Resolution:** Applied **SMOTE (Synthetic Minority Over-sampling Technique)** to address minority class imbalance.
- **Multi-Model Evaluation:** Trained and evaluated **Logistic Regression**, **Random Forest**, and **XGBoost** algorithms.
- **Feature Importance Analysis:** Extracted top factors driving churn using feature importance scores.

---

## 🛠️ Tech Stack & Libraries
- **Language:** Python 3.x
- **Environment:** Google Colab / Jupyter Notebook
- **Data Manipulation:** Pandas, NumPy
- **Machine Learning & Preprocessing:** Scikit-Learn, Imbalanced-Learn (SMOTE), XGBoost
- **Data Visualization:** Matplotlib, Seaborn

---

## 🚀 Model Performance Comparison

| Model | Evaluation Highlights |
| :--- | :--- |
| **Logistic Regression** | Baseline linear model for comparison |
| **Random Forest Classifier** | Robust ensemble method capturing non-linear patterns |
| **XGBoost Classifier** | High precision and recall with optimized gradient boosting |

*Key Evaluation Metrics:* Precision, Recall, F1-Score, and ROC-AUC Score.

---

## 💡 Key Business Insights
Based on Feature Importance analysis, the primary factors influencing customer churn are:
1. **Tenure:** Shorter tenure strongly correlates with higher churn risk.
2. **Contract Type:** Month-to-month contract holders churn significantly more than multi-year contract users.
3. **Monthly & Total Charges:** High monthly charges drive customers toward cancellation.
4. **Internet Service:** Fiber optic service users exhibit distinct churn patterns requiring retention focus.

---

## ⚙️ How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/abini-nk/telco-customer-churn.git](https://github.com/abini-nk/telco-customer-churn.git)
