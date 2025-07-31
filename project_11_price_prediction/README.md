# Project 11: Rusty Bargain – Used Car Price Prediction

## Objective
Build and evaluate machine learning models to predict the market price of used cars for the Rusty Bargain dealership. Compare models not only by prediction accuracy but also by training and prediction speed.

---

## Project Tasks

1. **Preprocess and Explore Data**
   - Clean missing values
   - Analyze key features (e.g., mileage, vehicle type, brand, power)
   - Encode categorical variables

2. **Model Building**
   - Linear Regression (baseline)
   - Decision Tree Regressor
   - Random Forest Regressor with tuning
   - LightGBM (boosted trees) with hyperparameter search
   - Optional: XGBoost / CatBoost (commented)

3. **Evaluation Metrics**
   - RMSE (Root Mean Squared Error)
   - Training and Prediction time

---

## Key Findings

- Linear Regression was fastest but least accurate.
- Random Forest offered a strong balance of accuracy and performance.
- LightGBM delivered comparable performance with faster training times.
- Boosted models require careful tuning for optimal performance.

---

## Tools & Libraries

- `pandas`, `numpy`
- `scikit-learn`
- `lightgbm`
- `matplotlib`, `seaborn`

---

## What I Learned

- How to compare model performance across different metrics
- RMSE as a preferred error metric in regression
- Time efficiency matters in production environments
- Tradeoffs between accuracy, training time, and complexity

---

## Project Structure

```bash
project_11_price_prediction/
├── notebooks/
│ └── project_11_rusty_bargain.ipynb
├── data/
│ └── car_data.csv
├── requirements.txt
└── README.md
