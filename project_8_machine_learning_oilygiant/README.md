# Project 8: Machine Learning in Business – OilyGiant

## Objective
OilyGiant, a mining company, wants to decide which of three regions to target for a new oil well. The goal is to build a **linear regression model** that predicts oil reserves and evaluates profitability and risk using **bootstrapping**.

---

## Business Constraints

- Only **Linear Regression** is allowed.
- Budget: $100 million to develop 200 wells.
- Revenue per 1,000 barrels = **$4.5k**
- Each region has 500 well locations; select the **top 200** based on predicted reserves.
- **Only regions with <2.5% risk of losses** are considered.
- Choose the region with **highest average profit** among those.

---

## Dataset

- `geo_data_0.csv`
- `geo_data_1.csv`
- `geo_data_2.csv`

Each file contains:
- `id`: Well identifier
- `f0`, `f1`, `f2`: Feature columns
- `product`: Volume of reserves in thousand barrels (target)

---

## Tools Used

- Python (pandas, numpy, matplotlib, scikit-learn)
- Linear Regression
- Bootstrap Sampling
- Confidence Intervals
- Risk Evaluation

---

## Process Overview

1. **Data Preprocessing**
   - Verified data types, checked for nulls
   - Visual inspection of features

2. **Modeling**
   - Trained `LinearRegression` models per region
   - Calculated RMSE, mean predictions

3. **Profit Function**
   - Selected top 200 predictions out of 500
   - Simulated profit based on budget and product yield

4. **Risk Analysis**
   - Bootstrapped 1000 samples for each region
   - Estimated:
     - Mean profit
     - 95% confidence interval
     - Risk of losses

---

## Findings

- **Region X** (replace with your result) had:
  - Highest expected profit
  - Risk of losses < 2.5%
- Recommended for oil well development

---

## Folder Structure 
```bash

project_8_machine_learning_oilygiant/
├── notebooks/
│   └── project_8_machine_learning_in_business.ipynb
├── data/
│   ├── geo_data_0.csv
│   ├── geo_data_1.csv
│   └── geo_data_2.csv
├── README.md
├── requirements.txt
