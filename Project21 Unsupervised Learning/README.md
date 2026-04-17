# Project 21 — Unsupervised learning (clustering)

## Problem statement

Discover **groups** in data **without** using a pre-labeled target. This notebook uses **synthetic 2D blobs** so you can compare how **K-means** and **DBSCAN** carve the plane differently.

## Notebook

- **`Clustring.ipynb`** — `sklearn.datasets.make_blobs` → `Feature_1` / `Feature_2`; **`StandardScaler`**; **elbow** plot (inertia vs **K**); **`KMeans`** (final `n_clusters=3`, plus an alternate `n_clusters=2`); **`DBSCAN`** (`eps=0.3`, `min_samples=5`); **Seaborn** scatterplots colored by cluster labels.

## Data

Synthetic only (**`make_blobs`**); no CSV required.

## Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn (`KMeans`, `DBSCAN`, `StandardScaler`, `make_blobs`), Jupyter Notebook
