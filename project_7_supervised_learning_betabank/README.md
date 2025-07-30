# Project 7: Supervised Learning – Beta Bank

## Objective
Beta Bank wants to reduce customer churn. Your job is to build a machine learning model that predicts whether a customer will leave the bank soon.

The goal is to achieve the highest possible **F1 score**, with a minimum passing threshold of **0.59**. In addition, the model’s **AUC-ROC score** must also be computed and evaluated.

---

## Dataset: `churn.csv`
Each row contains customer account information:

- `RowNumber` — index
- `CustomerId` — unique customer ID
- `Surname` — last name
- `CreditScore` — credit score
- `Geography` — country of residence
- `Gender` — gender
- `Age` — age
- `Tenure` — years as a customer
- `Balance` — account balance
- `NumOfProducts` — number of bank products used
- `HasCrCard` — has credit card? (1 = yes)
- `IsActiveMember` — account activity
- `EstimatedSalary` — monthly salary estimate
- `Exited` — target variable (1 = churned)

---

## Tools & Techniques
- Binary Classification
- Handling Imbalanced Data
- Feature Engineering
- GridSearchCV
- Evaluation: F1 Score, AUC-ROC
- scikit-learn

---

## 📈 Workflow

1. **Data Cleaning & Preprocessing**
   - Encoded categorical features
   - Standardized numerical features
   - Verified class imbalance

2. **Baseline Models**
   - Trained Logistic Regression, Decision Tree, and Random Forest
   - Evaluated performance without balancing

3. **Fixing Imbalance**
   - Strategy 1: Upsampling minority class
   - Strategy 2: Using `class_weight='balanced'`

4. **Final Evaluation**
   - Selected best model based on validation F1
   - Evaluated on test set (F1 & AUC-ROC)

---

## Results

- **Best model**: *Random Forest with balanced class weights*
- **Final F1 score**: **≥ 0.59** (threshold met)
- **AUC-ROC** confirmed model robustness
- **Recommendation**: Deploy model for churn retention campaigns

---

## Folder Structure

```bash
project_7_supervised_learning_betabank/
├── notebooks/
│   └── Project_7_Supervised_Learning_Beta_Bank.ipynb
├── data/
│   └── churn.csv
├── README.md
├── requirements.txt


