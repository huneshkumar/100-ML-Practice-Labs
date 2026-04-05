# Project 17 — Titanic: multi-classifier comparison

## Summary

Binary classification of **passenger survival** on the Seaborn **Titanic** dataset. After cleaning and encoding, several models are trained and compared with **accuracy**, **confusion matrices**, and **classification reports**.

## Notebook

- **`multi-models.ipynb`** — `sns.load_dataset('titanic')`, drop unused columns, features vs **`survived`**, train/test split, **feature scaling** for distance-based models. Classifiers: **logistic regression**, **k-NN** (`n_neighbors=5`), **Gaussian naive Bayes**, **decision tree** (`max_depth=5`), **SVC** (`C=1`).

## Data

No CSV in `datasets/` required; Titanic is loaded via Seaborn (same built-in dataset as in **Project 12**, with a broader model comparison here).

## Stack

Python, Pandas, NumPy, Seaborn, scikit-learn, Jupyter Notebook
