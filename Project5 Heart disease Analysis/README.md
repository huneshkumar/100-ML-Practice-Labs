# Project 5 — Heart Disease Analysis

## Problem Statement

Explore heart disease data to understand how clinical and demographic features (age, sex, chest pain type, resting BP, cholesterol, fasting blood sugar, ECG, max heart rate, exercise angina, ST slope, etc.) relate to the presence of heart disease. The goal is to identify which factors are most associated with the outcome and to summarize their distributions.

## Dataset

- **Source:** `../datasets/heart.csv`
- **Key columns:** Age, Sex, ChestPainType, RestingBP, Cholesterol, FastingBS, RestingECG, MaxHR, ExerciseAngina, Oldpeak, ST_Slope, HeartDisease (target)

## Analysis Performed

- **Understand dataset** — Load and review clinical heart disease indicators
- **Shape & info** — Dimensions and data types
- **Missing values** — Check for nulls
- **Target variable** — Distribution and balance of HeartDisease (0/1)
- **Categorical features** — Sex, ChestPainType, RestingECG, ExerciseAngina, ST_Slope
- **Numerical features** — Age, RestingBP, Cholesterol, FastingBS, MaxHR, Oldpeak
- **Feature engineering** — Risk bins or derived features if used
- **Correlation analysis** — Correlations among numerical variables and with target; heatmap
- **Visualization** — Histograms, boxplots (category vs numerical), countplots, heatmaps
- **Insights** — Factors most associated with heart disease and summary conclusions

## Key Insights (Summary)

- Balance of positive vs negative heart disease cases
- Impact of chest pain type, exercise angina, and ST slope on outcome
- Relationships between age, cholesterol, blood pressure, and heart disease
- Summary of variables that may be useful for prediction or screening

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
