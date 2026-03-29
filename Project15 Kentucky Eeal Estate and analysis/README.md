# Project 15 — Kentucky Real Estate (EDA + ML)

## Problem Statement

Analyze Kentucky real estate listings and predict **list price** (`listPrice`) using a full workflow: exploration, cleaning, feature engineering, scaling, **linear regression**, and **R²** evaluation on a held-out test set.

## Dataset

- **Source:** `../datasets/kentucky_real_estate.csv`
- **Scale:** ~8,500 listings (12 raw columns before cleaning)
- **Key columns:** type, sub_type, text, listPrice, sqft, stories, beds, baths, baths_full, baths_full_calc, garage, year_built

## Analysis Performed

1. **EDA** — Shape, `info`, `describe`, missing values, visualizations (e.g. price by type, garage).
2. **Data cleaning** — Drop duplicates; impute numerics with **median** and categoricals with `"Unknown"`; drop columns such as `text`, `sub_type`, `baths_full_calc` as implemented in the notebook.
3. **Feature engineering** — Price bins → **`category`**; one-hot **`type`** and **`category`**; **`house_age`** from `year_built`; drop `year_built` where applicable.
4. **Scaling** — `StandardScaler` on selected numeric features (dummy columns excluded per notebook).
5. **Modeling** — `train_test_split` (e.g. **33%** test, `random_state=42`), **`LinearRegression`**, `fit` / `predict`, **`r2_score`** on test predictions (example run in notebook: R² ≈ **0.77**).

## Key Insights (Summary)

- Strong baseline from engineered features (sqft, beds, baths, type, price tier, house age).
- Data quality: missingness and outliers in garage and extreme prices.
- Residual analysis and alternative models (e.g. regularized regression) can be added as next steps.

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (`StandardScaler`, `train_test_split`, `LinearRegression`, `r2_score`), Jupyter Notebook
