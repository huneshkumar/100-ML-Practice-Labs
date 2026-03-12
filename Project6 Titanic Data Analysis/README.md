# Project 6 — Titanic Data Analysis

## Problem Statement

Analyze Titanic passenger data to understand survival patterns. Explore how factors such as passenger class (Pclass), sex, age, number of siblings/spouses (SibSp), number of parents/children (Parch), fare, and embarkation port relate to survival. The goal is to describe who was more or less likely to survive and why.

## Dataset

- **Source:** `../datasets/titanic.csv`
- **Key columns:** PassengerId, Survived (target), Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, Embarked

## Analysis Performed

- **Understand dataset** — Load and inspect passenger and survival data
- **Shape & info** — Dimensions and data types
- **Missing values** — Handle missing Age, Cabin, Embarked
- **Target variable** — Distribution of Survived (0/1); overall survival rate
- **Categorical features** — Pclass, Sex, Embarked (counts and survival rates)
- **Numerical features** — Age, SibSp, Parch, Fare; summary stats and distributions
- **Feature engineering** — Title from name, family size, age groups if used
- **Correlation analysis** — Relationships between numerical variables and survival
- **Visualization** — Countplots, bar charts (survival by segment), boxplots, heatmaps
- **Insights** — Key factors associated with survival and narrative summary

## Key Insights (Summary)

- Survival rate by class, sex, and age group (“women and children first”)
- Effect of fare and cabin on survival (proxy for class)
- Impact of family size (SibSp, Parch) on survival
- Recommendations for further modeling or reporting

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
