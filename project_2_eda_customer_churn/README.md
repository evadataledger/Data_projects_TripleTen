# Project 2: Exploratory Data Analysis on Customer Churn

This project focuses on applying **exploratory data analysis (EDA)** to uncover insights about **customer churn** in a telecom dataset.
It was developed as part of the TripleTen Data Science Bootcamp and approved by TripleTen reviewers.

## Objective

To identify patterns and relationships that contribute to customer churn using visual and statistical EDA techniques. 
Understanding these patterns will allow businesses to take proactive action to reduce customer attrition.

## Dataset

The dataset contains anonymized customer records, including:
- Contract types (monthly, yearly)
- Service usage (internet, phone, streaming)
- Demographic data
- Monthly charges and total charges
- Churn status (target variable)

> Dataset is stored centrally in the `/datasets/` folder as `customer_churn_data.csv`

## Tools & Techniques 

- Python (`pandas`, `matplotlib`, `seaborn`)
- Jupyter Notebook
- Grouped comparisons, value counts, correlation heatmaps, and boxplots

## Key Insights

- Customers with month-to-month contracts are far more likely to churn.
- Higher monthly charges are associated with higher churn rates.
- Customers with shorter tenure tend to churn more frequently.
- Lack of certain services (like internet) also correlates with retention.

## What I learned

- How to ask targeted business questions and test hypotheses with EDA
- The power of visual storytelling for identifying business trends
- Applying correlation and grouped analysis to understand customer behavior
  
## Folder Structure

```bash
project_2_eda_customer_churn/
├── notebooks/
│   └── project_2_exploratory_data_analysis_.ipynb
├── requirements.txt
├── README.md
