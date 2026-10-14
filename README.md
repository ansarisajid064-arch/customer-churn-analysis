# Customer Churn Analysis

A churn analysis project exploring subscriber behavior across plan type,
subscription channel, state, and support interactions, built to identify
potential churn drivers and key business KPIs.

## Overview
Customer, subscription, and support data are read from a SQLite database
with SQL, then cleaned and merged in Pandas into one analysis-ready
dataset (20+ fields).

## Tools
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- SQL, SQLite
- Jupyter Notebook

## What this project does
- Reads three tables with SQL queries and merges them with Pandas
- Cleans data: fixes missing values, standardizes labels, corrects data types
- Engineers features: churn flag, customer tenure, complaint count,
  churn-risk segments (low / med / high)
- Analyzes churn by plan type, subscription channel, state, and month
- Investigates support escalations as a churn indicator
  (correlation 0.77 in this dataset)
- Calculates KPIs: churn rate, ARPU (~18.85), revenue at risk,
  average tenure (~1,548 days at original run)
- Visualizes findings with bar charts, a trend chart, and a correlation heatmap

## Note on dataset scale
This is a small practice dataset (~21 customers, 6 churned). Findings
illustrate the analytical approach and are not statistically robust.
The same pipeline would scale to larger datasets.

## How to run
1. Clone this repo
2. Install dependencies: `pip install pandas numpy matplotlib seaborn`
3. Keep `customer_churn.db` in the same folder as the notebook
4. Open `churn_analysis.ipynb` in Jupyter and run all cells


- `customer_churn.db`: SQLite source data
- `exported_churn_data.csv`: merged dataset created by the notebook
- `README.md`: this file
