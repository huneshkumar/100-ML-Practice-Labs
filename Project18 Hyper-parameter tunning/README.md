# Project 18 — Hyperparameter tuning & ensemble learning (Iris)

## Summary

Uses the classic **Iris** dataset (via Seaborn) for **multiclass classification**. One notebook (**`GridSearchCV.ipynb`**) tunes **k-NN** and **SVM** with **`GridSearchCV`** / **`RandomizedSearchCV`**. The other (**`EnsembleLearning.ipynb`**) walks through **EDA**, a **stacking** ensemble, and a **random forest** ensemble so you can compare approaches and test accuracies on the same split.

## Notebooks

### `GridSearchCV.ipynb`

- `sns.load_dataset('iris')`, features vs **species**, train/test split.
- **`GridSearchCV`** on **SVC** (`C`, `kernel`, etc.) and **k-NN** (`n_neighbors`, `weights`, `metric`, …).
- **`RandomizedSearchCV`** for an alternative search over the SVM space.

### `EnsembleLearning.ipynb`

1. **Load & EDA** — Iris from Seaborn; comments for basic EDA; **pair-style plots of features colored by species** (see notebook cells).
2. **Prepare labels** — **`LabelEncoder`** on **`species`** → `y_encoded`; **X** = numeric feature columns; **`train_test_split`** with **`stratify=y_encoded`**, `test_size=0.33`, `random_state=42`.
3. **Stacking** — **`StackingClassifier`** with base estimators: **`DecisionTreeClassifier`**, **`SVC`** (`probability=True`, RBF kernel, `random_state=42`), **`LogisticRegression`** (`max_iter=1000`); **`final_estimator=LogisticRegression`** (`max_iter=1000`); **`cv=5`**. Fit on train, predict on test, report **`accuracy_score`** (stored output in the notebook is on the order of **0.96**).
4. **Bagging-style forest (section `#bagging`)** — **`RandomForestClassifier`** with **`n_estimators=100`**, **`max_depth=None`**, **`random_state=42`**; same train/test split; **`accuracy_score`** on the test set for comparison with stacking.

`classification_report` is imported alongside `accuracy_score` if you extend evaluation.

## Data

Built-in **Iris** from Seaborn; no CSV in `datasets/` required.

## Stack

Python, Pandas, NumPy, Seaborn, Matplotlib, scikit-learn (`GridSearchCV`, `RandomizedSearchCV`, `StackingClassifier`, `RandomForestClassifier`, `LabelEncoder`, classifiers, metrics), Jupyter Notebook
