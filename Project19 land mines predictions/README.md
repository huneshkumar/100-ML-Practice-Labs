# Project 19 — Sonar: rock vs metal (mine) classification

## Problem statement

Sonar systems send pulses into the ground or water and record **energy at different frequencies**. The same pipeline of signals can reflect off **rock** or off **metal objects** (in this classic dataset, a **metal cylinder** is used as the positive class, often discussed in tutorials as a stand-in for “mine-like” metal).

**Goal:** learn a model that maps the **60 numeric sonar features** to a binary label so that, given a new sonar return profile, we can predict **R** (rock) vs **M** (metal). This supports exploration of **sensor-based binary classification**, **EDA across classes**, and **logistic regression** with clear **train vs test** accuracy.

**Why it matters (conceptually):** automated assistance for interpreting sonar returns could reduce manual review burden in **survey, robotics, or defense analytics** workflows. Any real operational demining or safety system would require **rigorous validation, domain sensors, regulations, and human oversight**—this notebook is **educational** only.

## Objectives

- Load and inspect **`sonar_data.csv`** (208 observations, 60 features + label).
- Compare **class balance** and **feature means** by class (`R` vs `M`).
- Train a **logistic regression** classifier with a **train/test split** (33% test, fixed random seed for reproducibility).
- Report **training and test accuracy** and demonstrate **prediction** on a sample 60-dimensional feature vector.

## Notebook

- **`Sonar_mine_prediction.ipynb`** — reads `../datasets/sonar_data.csv` (no header; columns named `1`…`61`, where **`61`** is the letter label).

## Dataset

| Item | Detail |
|------|--------|
| File | `datasets/sonar_data.csv` |
| Rows | 208 (classic sonar benchmark size) |
| Features | 60 continuous attributes (angles/frequency bands) |
| Target | **`61`**: `R` = rock, `M` = metal cylinder |

## Tech stack

Python, Pandas, NumPy, scikit-learn (logistic regression, train/test split, accuracy), Jupyter Notebook
