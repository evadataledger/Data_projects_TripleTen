# Project 9: Integrated ML Pipeline – Gold Recovery Optimization

## Objective
Build a machine learning model to predict gold recovery rates at different production stages of an industrial mining operation. The task required validating engineering recovery calculations, detecting data drift, and improving predictive performance with a custom evaluation metric (final sMAPE).

---

## Datasets Used

- `gold_recovery_train.csv` — Training set
- `gold_recovery_test.csv` — Test set (without targets)
- `gold_recovery_full.csv` — Source dataset with all parameters

---

## Tools & Techniques

- **Python**: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost
- **Model Evaluation**: sMAPE and weighted final sMAPE
- **Feature Engineering**: purification stage breakdowns, metal concentration analysis, outlier removal
- **Modeling**: RandomForest, XGBoost, Stacking
- **Drift Detection**: KDE plots, correlation shifts, visual EDA

---

## Final Results

- **Best Model**: Optimized **XGBoost**
- **Final Weighted sMAPE**: **10.0978**
- Stacked Model sMAPE: **10.2736**
- Random Forest w/ feature engineering: **11.6891**
- XGBoost w/ engineered features: **13.5741**

---

## 🔍 Key Insights

- Significant data drift detected in particle size distribution → selected tree-based models to mitigate
- sMAPE weighted as:  
  \> **25% rougher.output.recovery**  
  \> **75% final.output.recovery**
- Feature importance revealed that variables like `primary_cleaner.input.sulfate` and `rougher.input.feed_au` heavily influenced final recovery

---

## 📦 Folder Structure

```bash
project_9_gold_recovery_optimization/
├── notebooks/
│ └── Project_9_Gold_Recovery.ipynb
├── data/
│ ├── gold_recovery_train.csv
│ ├── gold_recovery_test.csv
│ └── gold_recovery_full.csv
├── requirements.txt
└── README.md

