# Project 18 — Hyperparameter tuning (Grid & Random search)

## Summary

Uses the classic **Iris** dataset (via Seaborn) for **multiclass classification**. A **k-NN** and **SVC** baseline are tuned with **`GridSearchCV`** (cross-validated grid search) and **`RandomizedSearchCV`** to pick stronger hyperparameters than hand-picked defaults.

## Notebook

- **`GridSearchCV.ipynb`** — `sns.load_dataset('iris')`, features vs **species**, train/test split; **`GridSearchCV`** on **SVC** (`C`, `kernel`, etc.) and **k-NN** (`n_neighbors`, `weights`, `metric`, …); **`RandomizedSearchCV`** for an alternative search over the SVM space.

## Data

Built-in **Iris** from Seaborn; no CSV in `datasets/` required.

## Stack

Python, Pandas, NumPy, Seaborn, scikit-learn (`GridSearchCV`, `RandomizedSearchCV`), Jupyter Notebook
