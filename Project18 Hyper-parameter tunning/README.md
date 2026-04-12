# Project 18 — Hyperparameter tuning & ensemble learning (Iris)

## Summary

Uses the classic **Iris** dataset (via Seaborn) for **multiclass classification**. One notebook tunes **k-NN** and **SVM** with **`GridSearchCV`** / **`RandomizedSearchCV`**. The other builds a **stacking ensemble** that combines a **decision tree**, **SVC**, and **logistic regression**, with a **logistic meta-learner** and cross-validated stacking folds.

## Notebooks

- **`GridSearchCV.ipynb`** — `sns.load_dataset('iris')`, features vs **species**, train/test split; **`GridSearchCV`** on **SVC** (`C`, `kernel`, etc.) and **k-NN** (`n_neighbors`, `weights`, `metric`, …); **`RandomizedSearchCV`** for an alternative search over the SVM space.

- **`EnsembleLearning.ipynb`** — Iris with **encoded** target, **stratified** `train_test_split` (`test_size=0.33`, `random_state=42`); **`StackingClassifier`** with base estimators **decision tree**, **SVC** (`probability=True`, RBF kernel), and **logistic regression**; **final estimator** logistic regression; **`cv=5`**; **test accuracy** via `accuracy_score`.

## Data

Built-in **Iris** from Seaborn; no CSV in `datasets/` required.

## Stack

Python, Pandas, NumPy, Seaborn, scikit-learn (`GridSearchCV`, `RandomizedSearchCV`, `StackingClassifier`, classifiers, metrics), Jupyter Notebook
