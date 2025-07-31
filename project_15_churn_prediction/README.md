# Project 15: Churn Prediction – Interconnect Telecom

## Objective
Build a predictive model to identify customers at risk of churning (leaving the telecom service). This enables **Interconnect Telecom** to proactively retain users with targeted incentives.

---

## Dataset Overview
Four datasets were provided and merged based on `customerID`:
- `contract.csv` — contract info
- `personal.csv` — customer demographics
- `internet.csv` — internet services used
- `phone.csv` — phone service details

> **Target Feature**: `EndDate == 'No'` (customer is still active)

---

## Tasks Completed
- Combined all tables on `customerID`
- Cleaned & encoded categorical variables
- Explored service usage trends and contract types
- Handled class imbalance
- Trained multiple models: Logistic Regression, Random Forest, Gradient Boosting
- Evaluated models with:
  - AUC-ROC (primary metric)
  - Accuracy (secondary metric)

---

## Model Performance

| Model               | AUC-ROC Score |
|---------------------|---------------|
| Logistic Regression | ~0.83         |
| Random Forest       | ~0.86         |
| Gradient Boosting   | **0.88+**   |

 **Final Model**: Gradient Boosting  
 **Final AUC-ROC**: **≥ 0.88** (6 SP Score Tier Achieved)

---

## Tools Used
- Python (pandas, numpy)
- scikit-learn
- matplotlib, seaborn
- CatBoost / XGBoost (optional for boosting)

---

## Folder Structure

```bash
project_15_churn_prediction/
├── notebooks/
│   └── Project_15_Interconnect_Churn.ipynb
├── README.md
├── requirements.txt
