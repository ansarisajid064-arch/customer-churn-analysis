Customer Churn Analysis

A churn analysis project exploring subscriber behavior across plan type, contract type, state, and support interactions, built to identify potential churn drivers and key business KPIs.

Overview

This project integrates customer, subscription, and support data from a relational database (PostgreSQL/SQLite) into a unified dataset for analysis. It focuses on identifying patterns in customer churn, quantifying business metrics like ARPU and revenue at risk, and visualizing findings for decision-making.

Tools & Libraries
Python (Pandas, NumPy)
SQL (PostgreSQL, SQLite)
Matplotlib & Seaborn for visualization
Jupyter Notebook
What This Project Does
Merges customer, subscription, and support tables using SQL joins and Pandas, consolidating 20+ fields
Cleans data: handles missing values, standardizes inconsistent categorical labels, encodes categorical variables
Engineers features: churn flag, customer tenure, and churn-risk segments (Low/Medium/High)
Analyzes churn across plan type, subscription type, state, and tenure using pivot-style aggregations
Investigates support escalations as a potential churn indicator (correlation observed: 0.77, in this dataset)
Calculates KPIs: churn rate, ARPU (~18.85), revenue at risk, average tenure (~1,548 days)
Visualizes findings with correlation heatmaps and segment/trend charts
Note on Dataset Scale

This project uses a small practice dataset (~21 customers) for learning purposes. Correlation and segment findings are illustrative of the analytical approach rather than statistically robust conclusions — the same pipeline would scale to larger, real-world datasets.

How to Run
Clone this repo
Install dependencies: pip install pandas numpy matplotlib seaborn
Open churm_analysis.ipynb in Jupyter
Run all cells top to bottom
Files
churm_analysis.ipynb — main analysis notebook
README.md — this file
