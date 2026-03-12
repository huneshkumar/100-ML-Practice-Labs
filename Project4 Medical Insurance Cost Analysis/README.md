# Project 4 — Medical Insurance Cost Analysis

## Problem Statement

Analyze medical insurance data to understand how factors such as age, sex, BMI, number of children, smoking status, and region influence insurance charges. The goal is to identify which variables most affect premium costs and to describe their relationships.

## Dataset

- **Source:** `../datasets/insurance.csv`
- **Key columns:** age, sex, bmi, children, smoker, region, charges (target)

## Analysis Performed

- **Understand dataset** — Load and inspect insurance records
- **Shape & info** — Dimensions and data types
- **Missing values** — Check for nulls
- **Target variable** — Distribution and summary of `charges`
- **Categorical features** — sex, smoker, region (counts and impact on charges)
- **Numerical features** — age, bmi, children; summary stats and distributions
- **Feature engineering** — Bins or segments if used (e.g. age groups, BMI categories)
- **Correlation analysis** — Correlation of numerical variables with charges; heatmap
- **Visualization** — Histograms, boxplots (category vs charges), scatter plots, heatmaps
- **Insights** — Main drivers of insurance cost and recommendations

## Key Insights (Summary)

- Strong effect of smoking and age on charges
- Impact of BMI and region on premiums
- Distribution of charges by sex and number of children
- Recommendations for understanding or predicting insurance costs

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
