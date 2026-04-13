# Project 18 — Hyperparameter tuning & ensemble learning (Iris)

## Summary

Uses the classic **Iris** dataset (via Seaborn) for **multiclass classification**. **`GridSearchCV.ipynb`** tunes **k-NN** and **SVM**. **`EnsembleLearning.ipynb`** combines **EDA**, a **stacking** ensemble, a **random forest**, and **boosting** models (**AdaBoost**, **gradient boosting**, **XGBoost**), with **test accuracy** for each fit.

## Notebooks

### `GridSearchCV.ipynb`

- `sns.load_dataset('iris')`, features vs **species**, train/test split.
- **`GridSearchCV`** on **SVC** and **k-NN**; **`RandomizedSearchCV`** on SVM.

### `EnsembleLearning.ipynb`

1. **Load & EDA** — Iris from Seaborn; plots of features **colored by species**.
2. **Prepare labels** — **`LabelEncoder`** on **`species`** → `y_encoded`; **X** = numeric features; **`train_test_split`** with **`stratify=y_encoded`**, `test_size=0.33`, `random_state=42`.
3. **Stacking** — **`StackingClassifier`**: bases **`DecisionTreeClassifier`**, **`SVC`** (`probability=True`, `random_state=42`), **`LogisticRegression`** (`max_iter=1000`); **`final_estimator=LogisticRegression`** (`max_iter=1000`); **`cv=5`**. Test **`accuracy_score`**.
4. **`#bagging`** — **`RandomForestClassifier`**: `n_estimators=100`, `max_depth=None`, `random_state=42`. Test accuracy.
5. **`#adaboost`** — **`AdaBoostClassifier`**: `n_estimators=100`, `random_state=42`. Test accuracy.
6. **Gradient boosting (sklearn)** — **`GradientBoostingClassifier`**: `n_estimators=100`, `learning_rate=0.1`, `random_state=42`. Test accuracy.
7. **XGBoost** — Notebook uses **`!pip install xgboost`** then **`XGBClassifier`**: `n_estimators=100`, `learning_rate=0.1`, `max_depth=3`, `use_label_encoder=False`, `eval_metric='mlogloss'`, `random_state=42`. Test accuracy.

`classification_report` is imported with `accuracy_score` for optional extensions.

## Dependencies

- Base stack: see repo **Getting Started** (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `jupyter`).
- **`pip install xgboost`** (or run the install cell) before the **XGBClassifier** section in **`EnsembleLearning.ipynb`**.

## Data

Built-in **Iris** from Seaborn; no CSV in `datasets/` required.

## Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, **XGBoost**, Jupyter Notebook
