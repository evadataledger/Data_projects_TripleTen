# Project 12: Time Series Forecasting – Sweet Lift Taxi Company

## Objective
Build a predictive model to forecast the number of taxi orders for the next hour using historical airport order data. This helps Sweet Lift attract more drivers during peak hours.

---

## Problem Context
Sweet Lift collected data on hourly taxi orders. Your goal:  
  Predict hourly demand and ensure the model achieves **RMSE ≤ 48** on the test set.

---

## Project Workflow

1. **Data Preparation**
   - Resampled raw data into hourly time series
   - Handled missing values and visualized trends, seasonality, and stationarity

2. **Feature Engineering**
   - Created lag features
   - Added rolling means and time-based features

3. **Model Training**
   - Linear Regression (Baseline)
   - Random Forest Regressor
   - CatBoost Regressor
   - LightGBM
   - Final tuned model selection based on validation set

4. **Evaluation**
   - Used RMSE as the primary metric
   - Split dataset with 10% reserved for test set
   - Final RMSE:  **below 48 threshold**

---

## Tools & Libraries
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`
- `LightGBM`, `CatBoost`

---

## Key Insight
Lag features and rolling averages significantly improved the model’s ability to capture seasonality and short-term fluctuations in demand.

---

## What I Learned
- Practical time series forecasting with machine learning
- Feature engineering for time-based trends
- Real-world model deployment scenarios using RMSE thresholding

---

## Project Structure

```bash 
project_12_time_series/
├── notebooks/
│ └── project_12_sweetlift_time_series.ipynb
├── data/
│ └── README.md (dataset >100MB not included)
├── requirements.txt
└── README.md
