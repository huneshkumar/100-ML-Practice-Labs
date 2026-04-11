# Project 20 — Diabetes onset prediction (binary classification)

## Problem statement

Using tabular **clinical and demographic** measurements, we want to predict whether a patient is labeled with **diabetes onset** (`Outcome` = 1) or not (0). This is a standard **binary classification** learning problem on a small, well-known dataset (often called **Pima Indians Diabetes** in tutorials).

**Important:** This notebook is for **education and portfolio practice** only. It is **not** a medical device, not validated for any population, and must **not** be used for real diagnosis or treatment decisions.

## Objectives

- Load **`diabetes.csv`** and explore **class balance** and **feature means** by `Outcome`.
- Build **X** (all columns except `Outcome`) and **y** (`Outcome`).
- Apply **`StandardScaler`** so SVM sees comparable feature scales.
- Split into train/test (33% test, `random_state=42`).
- Tune **`sklearn.svm.SVC`** with **`GridSearchCV`** (e.g. over `C` and `kernel`).
- Measure **train and test accuracy** and run a **single-row prediction** example.
- Save the **best estimator** and **scaler** with **`joblib`** under **`models/`** (create that folder by running the export cells, or add it manually if needed).

## Notebook

- **`Diabetese_prediction.ipynb`** — end-to-end pipeline and persistence paths `./models/diabetic_model.pkl` and `./models/scaler.pkl`.

## Dataset

| File | `datasets/diabetes.csv` |
| Rows | 768 |
| Target | **`Outcome`** (0 / 1) |
| Features | e.g. Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age |

## Stack

Python, Pandas, NumPy, scikit-learn (SVM, `GridSearchCV`, `StandardScaler`, metrics), joblib, Jupyter Notebook
