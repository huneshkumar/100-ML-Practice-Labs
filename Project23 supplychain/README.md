# Project 23 — Supply chain EDA

## Problem Statement

Explore a large supply-chain / e-commerce order dataset to understand shipping performance, delivery risk, sales and profit patterns, customer and product attributes, and how order and shipping dates behave after cleaning.

## Dataset

- **Source:** `../datasets/supply_chain_data.csv` (load with **`encoding='latin-1'`** so mixed encodings in text columns do not fail)
- **Scope:** Wide transactional table (orders, line items, customer and order geography, product details, payment type, delivery status, **late delivery risk**, and timestamps)

## Analysis Performed

- Load CSV; inspect shape, dtypes, and missing values.
- Parse date columns with **`pd.to_datetime`** and **`errors='coerce'`** where needed.
- Drop redundant or unused columns after review.
- Numerical summaries (**`describe`**) and categorical distributions.
- Visualizations with **Matplotlib** / **Seaborn** (e.g. **viridis** palette).

## Key Insights (Summary)

- Document patterns in delivery timeliness, regional or category slices, and relationships between sales, discounts, and profit where the notebook derives them.

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
