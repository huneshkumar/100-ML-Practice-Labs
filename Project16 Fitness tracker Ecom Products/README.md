# Project 16 — Fitness Tracker E-commerce EDA & Modeling

## Problem Statement

Explore smartwatch and fitness-tracker style **e-commerce product** data to understand price, features, brands, and relationships between variables. The workflow follows business/DS steps from `docs/doc.txt` (framing, collection, preprocessing, analysis, visualization, then modeling).

## Notebooks & data flow

1. **`Fitness_tracker_ecommerce.ipynb`** — EDA on `../datasets/smartwatches.csv`: drop index column **`Unnamed: 0`**, **ydata-profiling** on a train split, univariate plots (**Seaborn** `histplot` with KDE, **boxplot**), multivariate **pairplot**, correlation **heatmap**, then feature prep with **`pd.get_dummies`** on **`Brand`** and **`Dial Shape`**. Writes **`final_watch_data.csv`** in this project folder (regenerate by running the notebook if you change upstream data).

2. **`Model_creation.ipynb`** — Loads **`final_watch_data.csv`**, predicts **`Discount Price`** from the remaining numeric and one-hot columns. **Train/test split** (33% test, `random_state=42`). Models: **linear regression**, **decision tree**, **random forest**; **R²** on held-out test (and **5-fold `cross_val_score`** with `scoring='r2'`). Requires `scikit-learn`.

## Datasets

- **Source CSV:** `../datasets/smartwatches.csv`
- **Modeling table:** `final_watch_data.csv` (produced by the EDA notebook; committed for convenience)
- **Alternates in repo:** `../datasets/Fitness_trackers.csv`, `../datasets/Fitness_trackers_updated.csv` for extensions or swapping sources

## Key insights (summary)

- Distributions of price, ratings, and specs; brand and dial-shape patterns after encoding.
- Correlations among numeric features (heatmap / pairplot).
- **Discount Price** is predictable from engineered features; compare linear, tree, and ensemble test **R²** in the modeling notebook.

## Tech stack

Python, Pandas, NumPy, Matplotlib, Seaborn, ydata-profiling, scikit-learn, Jupyter Notebook
