# Project 3: Statistical Data Analysis – Megaline Plans

## Objective

Analyze which of Megaline’s prepaid plans — Surf or Ultimate — generates more monthly revenue, based on 500 clients’ call, message, and data usage.

## Key Questions

- How do Surf and Ultimate users behave?
- What are the average monthly usage patterns?
- Which plan results in higher revenue?
- Do regional users (e.g., NY-NJ) behave differently?

## Data Sources

- `megaline_calls.csv`
- `megaline_internet.csv`
- `megaline_messages.csv`
- `megaline_users.csv`
- `megaline_plans.csv`

## Techniques Used

- Data cleaning (NaNs, dtypes)
- Aggregation (groupby, monthly totals)
- Revenue calculation logic
- Hypothesis Testing (t-tests)
- Visualization (histograms, bar plots)

## Outcome

Surf appears more cost-efficient for light users, but Ultimate offers stability for heavy users. Hypothesis tests confirm revenue difference.

## Folder Structure

```bash
project_3_statistical_data_analysis/
├── notebooks/
│   └── project_3_statistical_data_analysis_(clean).ipynb
├── data/
│   └── megaline_calls.csv
│   └── megaline_internet.csv
│   └── megaline_messages.csv
│   └── megaline_plans.csv
│   └── megaline_users.csv
├── README.md
├── requirements.txt

