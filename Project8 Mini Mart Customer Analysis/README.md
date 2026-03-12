# Project 8 — Mini Mart Customer Analysis

## Problem Statement

Analyze mini mart customer data to understand how demographics (age, gender), income, membership tenure, and spending score relate to each other. The goal is to identify customer segments and patterns (e.g. high spenders, loyal members) to support targeting and loyalty strategies.

## Dataset

- **Source:** In-notebook (synthetic data); no external CSV in `datasets/`
- **Key columns:** customer_id, age, gender, annual_income, spending_score, membership_years

## Analysis Performed

- **Understand dataset** — Load and inspect customer profile data (created in notebook)
- **Shape & info** — Dimensions and data types
- **Missing values** — Check for nulls (if data is extended)
- **Target/focus** — Spending score or segment as main outcome of interest
- **Categorical features** — gender (counts and comparison by segment)
- **Numerical features** — age, annual_income, spending_score, membership_years
- **Feature engineering** — Segments (e.g. by income or spending), loyalty tiers if used
- **Correlation analysis** — Relationships between income, spending, age, membership
- **Visualization** — Histograms, scatter plots (income vs spending), boxplots, countplots
- **Insights** — Customer segments and recommendations for the mini mart

## Key Insights (Summary)

- Relationship between annual income and spending score
- Distribution of customers by age, gender, and membership years
- Identification of high-value or high-potential segments
- Suggestions for promotions or loyalty programs

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
