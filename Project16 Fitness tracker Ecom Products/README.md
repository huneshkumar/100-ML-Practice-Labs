# Project 16 — Fitness Tracker E-commerce EDA

## Problem Statement

Explore smartwatch and fitness-tracker style **e-commerce product** data to understand price, features, brands, and relationships between variables. The workflow follows business/DS steps: problem framing, data collection, preprocessing, analysis, and visualization (see `docs/doc.txt`).

## Dataset

- **Primary (notebook):** `../datasets/smartwatches.csv`
- **Also in repo:** `Fitness_trackers.csv`, `Fitness_trackers_updated.csv` in `datasets/` for extensions or alternate analyses.

## Analysis Performed

- Load data with Pandas; remove stray **Unnamed** columns where applicable.
- **ydata-profiling** for an automated profile report (install via `pip install ydata-profiling`).
- **Univariate:** histograms, density-style plots, box-and-whisker plots.
- **Multivariate:** correlation heatmaps, scatter plots.
- Optional next steps from `docs/doc.txt`: modeling, evaluation, deployment.

## Key Insights (Summary)

- Product and price distributions across brands or categories.
- Correlations between numeric features (e.g. price vs. specs).
- Data quality issues surfaced by profiling and manual checks.

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, ydata-profiling, Jupyter Notebook
