# Project 12 — ML: Logistic Regression — Titanic Survival Prediction

## Problem Statement

Build a **logistic regression** (classification) model to predict Titanic passenger survival (survived: 0/1) using features such as class, sex, age, sibsp, parch, fare, embarked, and derived columns. The goal is to identify which factors predict survival and to evaluate classification performance.

## Dataset

- **Source:** Loaded in the notebook via **Seaborn** — `sns.load_dataset('titanic')` (built-in dataset, not the repo's `titanic.csv`).
- **Key columns:** survived (target), pclass, sex, age, sibsp, parch, fare, embarked, class, who, adult_male, deck, embark_town, alive, alone.

## Analysis Performed

- Load Titanic data with Seaborn; explore shape, info, missing values.
- EDA and visualizations; encode categoricals (e.g. sex, embarked) for modeling.
- Prepare features (X) and target (y); train/test split.
- Fit **LogisticRegression**; evaluate with accuracy, confusion matrix, classification report.
- Interpret coefficients and summarize insights.

## Key Insights (Summary)

- Which features most influence survival (e.g. sex, class, fare).
- Model performance (accuracy, precision, recall) and confusion matrix.
- Practical takeaways for understanding survival factors.

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn (LogisticRegression, train_test_split, metrics), Jupyter Notebook
