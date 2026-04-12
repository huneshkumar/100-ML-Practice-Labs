# EDA Projects

A collection of **Exploratory Data Analysis (EDA)** and **Machine Learning (ML)** projects (regression and classification) across **20** themed folders, demonstrating data cleaning, visualization, insight extraction, and prediction using Python, Pandas, and visualization libraries.

---

## Contents

- [Overview](#overview)
- [EDA Checklist](#eda-checklist)
- [Chart Selection Guide](#chart-selection-guide)
- [Projects](#projects)
- [Repository Structure](#repository-structure)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Datasets](#datasets)
- [Usage](#usage)

---

## Overview

This repository contains hands-on EDA and ML projects built with Jupyter notebooks. EDA projects focus on real-world datasets with data loading, quality checks, visualization, and insights. ML projects (**9–12**, **15**–**20**) add regression or classification models, train/test evaluation, and metrics (e.g. R², accuracy). **Project 18** covers **hyperparameter search** (`GridSearchCV`, `RandomizedSearchCV` on Iris) and **stacking ensembles** (`StackingClassifier` with tree, SVM, and logistic base learners). **Project 19** is a classic **sonar** binary classification task (rock vs metal). **Project 20** predicts **diabetes onset** (**Outcome**) from clinical features using **scaled** inputs and **SVM** with **`GridSearchCV`**. Each project folder has its own **README.md** with problem statement, dataset description, analysis steps, and key insights.

---

## EDA Checklist

Each project in this repository follows a structured exploratory data analysis workflow:

| # | Step | Description |
|---|------|-------------|
| 1 | **Understand dataset** | Load data, review columns, and get familiar with the domain. |
| 2 | **Check shape and info** | Inspect dimensions, dtypes, and memory usage. |
| 3 | **Check missing values** | Identify and handle nulls or incomplete records. |
| 4 | **Analyze target variable** | Explore distribution and patterns in the target/outcome. |
| 5 | **Analyze categorical features** | Counts, value distributions, and mode for categorical columns. |
| 6 | **Analyze numerical features** | Summary stats, distributions, and outliers for numeric columns. |
| 7 | **Feature engineering** | Create or transform features to support analysis or modeling. |
| 8 | **Correlation analysis** | Examine relationships between numerical variables. |
| 9 | **Visualization** | Charts and plots to communicate findings. |
| 10 | **Write insights** | Document key takeaways and recommendations. |

---

## Chart Selection Guide

Choose the right visualization based on your data types:

| Data Type | Chart |
|-----------|-------|
| Numerical distribution | Histogram |
| Numerical vs Numerical | Scatter plot |
| Category vs Numerical | Boxplot / Bar chart |
| Category counts | Countplot |
| Multiple variables | Heatmap |

---

## Projects

| Project | Description | Dataset |
|--------|-------------|---------|
| **Project 1 — Books Sales** | Analysis of book sales, ratings, genres, and publisher performance. | `Books_Data_Clean.csv` |
| **Project 2 — Shopping Behaviour** | Exploration of customer shopping trends and purchasing patterns. | `shopping_trends.csv` |
| **Project 3 — Netflix Movies & TV Shows** | Analysis of Netflix content distribution, genres, and growth over time. | `netflix_titles.csv` *(add file to `datasets/` if missing)* |
| **Project 4 — Medical Insurance Cost** | Analysis of medical insurance costs and factors affecting premiums. | `insurance.csv` |
| **Project 5 — Heart Disease Analysis** | EDA of heart disease indicators and related health metrics. | `heart.csv` |
| **Project 6 — Titanic Data Analysis** | Analysis of Titanic passenger data and survival patterns. | `titanic.csv` |
| **Project 7 — Air Ticket Price Analysis** | Analysis of airline ticket prices and pricing factors. | `airline_ticket_prices_dataset.csv` |
| **Project 8 — Mini Mart Customer Analysis** | Analysis of mini mart customer behavior and purchasing patterns. | In-notebook data |
| **Project 9 — ML: Insurance Charges Prediction** | Linear regression model to predict medical insurance charges from age, BMI, smoker, etc. | `insurance.csv` |
| **Project 10 — ML: Ford Car Price Prediction** | Linear regression model to predict used Ford car prices from model, year, mileage, transmission, fuel type, etc. | `ford.csv` |
| **Project 11 — ML: House Price Prediction** | Linear regression model to predict median house prices (Boston Housing) from CRIM, RM, LSTAT, etc. | OpenML (see notebook) |
| **Project 12 — ML: Titanic Survival (Logistic Regression)** | Logistic regression model to predict passenger survival from class, sex, age, fare, etc. | Seaborn (titanic) |
| **Project 13 — Bollywood Movies EDA** | EDA on Bollywood movies: genre, release period, budget, revenue, screens, remakes, and franchises. | `Bollywood_movies.csv` |
| **Project 14 — General Election 1970–2024** | EDA on NA constituency–level election data: parties, votes, turnout, provinces, and trends over time. | `general_election_1970to2024.csv` |
| **Project 15 — Kentucky Real Estate** | Full pipeline: EDA, cleaning, feature engineering (price tiers, one-hot encoding, `house_age`), scaling, then **linear regression** to predict **list price** (`listPrice`); train/test split and **R²** evaluation. | `kentucky_real_estate.csv` |
| **Project 16 — Fitness Tracker E-commerce** | **EDA:** `smartwatches.csv`, drop index column, **ydata-profiling**, histograms (KDE), boxplots, pairplot, correlation heatmap; one-hot **Brand** / **Dial Shape** → **`final_watch_data.csv`**. **ML:** linear regression, decision tree, and random forest to predict **Discount Price**; R² and 5-fold CV (`Model_creation.ipynb`). | `smartwatches.csv` → `Project16 Fitness tracker Ecom Products/final_watch_data.csv` |
| **Project 17 — Titanic: multi-classifier comparison** | **Classification:** Seaborn **Titanic**; clean/drop columns, encode features, train/test split; compare **logistic regression**, **k-NN** (`n_neighbors=5`, scaled features), **Gaussian naive Bayes**, **decision tree** (`max_depth=5`), and **SVC** (`C=1`); **accuracy**, confusion matrix, classification report (`multi-models.ipynb`). | Seaborn `sns.load_dataset('titanic')` |
| **Project 18 — Hyperparameter tuning & ensembles** | **Iris** (Seaborn): **`GridSearchCV.ipynb`** — **k-NN** and **SVC** baselines, **`GridSearchCV`** (5-fold CV) on SVM and k-NN, **`RandomizedSearchCV`** on SVM. **`EnsembleLearning.ipynb`** — label-encoded species, stratified split, **`StackingClassifier`** (base: **decision tree**, **SVC** `probability=True`, **logistic regression**; meta: **logistic regression**, `cv=5`) and **test accuracy**. | Seaborn `sns.load_dataset('iris')` |
| **Project 19 — Sonar: mine vs rock classification** | **Binary classification:** 60 sonar frequency-energy features plus label **R** (rock) vs **M** (metal); EDA, train/test split, **logistic regression**, train and test **accuracy**, and a worked **prediction** example (`Sonar_mine_prediction.ipynb`). | `sonar_data.csv` |
| **Project 20 — ML: Diabetes prediction** | **Binary classification (Pima-style):** load **`diabetes.csv`**, EDA (`Outcome` balance, group means), **`StandardScaler`** on features, train/test split, **`GridSearchCV`** over **SVC** (`C`, `kernel`), train/test **accuracy**, sample inference, **`joblib`** export of fitted model and scaler to **`models/`** (`Diabetese_prediction.ipynb`). | `diabetes.csv` |

Each project folder contains a **README.md** with problem statement, dataset details, analysis steps, and key insights (**Projects 9–12 and 15–20** include trained models, tuning, or evaluation).

---

## Repository Structure

```
.
├── datasets/
│   ├── Books_Data_Clean.csv
│   ├── shopping_trends.csv
│   ├── insurance.csv
│   ├── diabetes.csv
│   ├── heart.csv
│   ├── titanic.csv
│   ├── airline_ticket_prices_dataset.csv
│   ├── ford.csv
│   ├── Bollywood_movies.csv
│   ├── general_election_1970to2024.csv
│   ├── kentucky_real_estate.csv
│   ├── smartwatches.csv
│   ├── sonar_data.csv
│   ├── Fitness_trackers.csv
│   └── Fitness_trackers_updated.csv
├── Project1 Books Sales/
│   ├── Books.ipynb
│   └── README.md
├── Project2 Shopping Behavioure/
│   ├── customerShoppingBehavioure.ipynb
│   └── README.md
├── Project3 Netflix Movies & TV Shows Analysis/
│   ├── NetflixAnalysis.ipynb
│   └── README.md
├── Project4 Medical Insurance Cost Analysis/
│   ├── insurance.ipynb
│   └── README.md
├── Project5 Heart disease Analysis/
│   ├── HeartAnalysis.ipynb
│   └── README.md
├── Project6 Titanic Data Analysis/
│   ├── titanicAnalysis.ipynb
│   └── README.md
├── Project7 Air Ticket Price Analysis/
│   ├── AirTicketPriceAnalysis.ipynb
│   └── README.md
├── Project8 Mini Mart Customer Analysis/
│   ├── miniMartCustomerAnalysis.ipynb
│   └── README.md
├── Project9 ML-Liner-regression-Insurance charges predections/
│   ├── insurance.ipynb
│   └── README.md
├── Project10 ML Ford Car Price predections/
│   ├── Ford_Price_Predection.ipynb
│   └── README.md
├── Project11 ML House Price Predection/
│   ├── housePircePredection.ipynb
│   └── README.md
├── Project12 ML Logestic-regression Titanic survival/
│   ├── Untitled.ipynb
│   └── README.md
├── Project13 Bollywood Movies EDA/
│   ├── Bollywood Movies Eda.ipynb
│   └── README.md
├── Project14 General Election 1970 to 2024/
│   ├── Election_1970_to_2024.ipynb
│   └── README.md
├── Project 15 Kentucky Eeal Estate and analysis/
│   ├── kentucky_real_estate.ipynb
│   └── README.md
├── Project16 Fitness tracker Ecom Products/
│   ├── Fitness_tracker_ecommerce.ipynb
│   ├── Model_creation.ipynb
│   ├── final_watch_data.csv
│   ├── docs/
│   │   └── doc.txt
│   └── README.md
├── Project17 Logistic-regression/
│   ├── multi-models.ipynb
│   └── README.md
├── Project18 Hyper-parameter tunning/
│   ├── GridSearchCV.ipynb
│   ├── EnsembleLearning.ipynb
│   └── README.md
├── Project19 land mines predictions/
│   ├── Sonar_mine_prediction.ipynb
│   └── README.md
├── Project20 ML Diabetes Predictions/
│   ├── Diabetese_prediction.ipynb
│   └── README.md
└── readme.md
```

---

## Tech Stack

- **Python 3**
- **Pandas** — data manipulation and analysis
- **NumPy** — numerical operations
- **Matplotlib** — static visualizations
- **Seaborn** — statistical visualizations
- **Jupyter Notebook** — interactive analysis
- **Scikit-learn** — for Projects 9–12 and **15**–**20** (linear/logistic regression, k-NN, naive Bayes, SVM, tree/ensemble models, **`StackingClassifier`**, **`GridSearchCV`** / **`RandomizedSearchCV`**, train/test split, scaling, metrics, OpenML where used, classification/regression evaluation)
- **Joblib** — used in **Project 20** to persist the tuned model and scaler (run the notebook to create the `models/` files)
- **ydata-profiling** — optional for **Project 16** (automated EDA HTML reports)

---

## Getting Started

### Prerequisites

- Python 3.8 or higher  
- Jupyter (or JupyterLab)

### Setup

1. **Clone or download** this repository.

2. **Create a virtual environment** (recommended):

   ```bash
   python -m venv venv
   venv\Scripts\activate    # Windows
   # source venv/bin/activate  # macOS/Linux
   ```

3. **Install dependencies**:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

   For **Project 16** (fitness tracker e-commerce EDA), also install:

   ```bash
   pip install ydata-profiling
   ```

4. **Launch Jupyter**:

   ```bash
   jupyter notebook
   ```

5. Open any `.ipynb` file from the project folders. For CSV-based projects, ensure paths point to the `datasets/` folder when loading data (e.g. `../datasets/filename.csv` from a project folder).

---

## Datasets

- **Books_Data_Clean.csv** — Book metadata, ratings, sales, and publisher information.
- **shopping_trends.csv** — Customer shopping and trend data for behaviour analysis.
- **insurance.csv** — Medical insurance cost data for cost and premium analysis.
- **diabetes.csv** — Pima Indians Diabetes–style records (768 rows): glucose, blood pressure, BMI, age, pedigree, etc., and binary **`Outcome`**; **Project 20** loads `../datasets/diabetes.csv` in `Diabetese_prediction.ipynb`.
- **heart.csv** — Heart disease and cardiovascular health indicators for analysis.
- **titanic.csv** — Titanic passenger and survival data for demographic and outcome analysis.
- **airline_ticket_prices_dataset.csv** — Airline ticket pricing data for price and factor analysis.
- **ford.csv** — Used Ford car listings (model, year, mileage, transmission, fuel type, tax, mpg, engine size) for price prediction.
- **Bollywood_movies.csv** — Bollywood film metadata, budget, revenue, genre, and release attributes for EDA.
- **general_election_1970to2024.csv** — General election records (1970–2024): NA constituencies, parties, candidates, votes, provinces, and regional fields.
- **kentucky_real_estate.csv** — Kentucky real estate listings (~8.5k rows): list price, sqft, beds, baths, property type, garage, year built, listing text; **Project 15** uses it for EDA, feature engineering, and **linear regression** on list price.
- **smartwatches.csv** — Smartwatch / wearable e-commerce product attributes; **Project 16** loads this in `Fitness_tracker_ecommerce.ipynb` and exports **`Project16 Fitness tracker Ecom Products/final_watch_data.csv`** (one-hot encoded features) for **`Model_creation.ipynb`**.
- **sonar_data.csv** — Classic **sonar** dataset (~208 rows): **60** numeric attributes (return strengths) and a label column **R** / **M** (rock vs metal); **Project 19** loads it from `../datasets/sonar_data.csv` in `Sonar_mine_prediction.ipynb`.
- **Fitness_trackers.csv** / **Fitness_trackers_updated.csv** — Additional fitness-tracker product data in `datasets/` (use if you extend the notebook or swap the data source).

*Project 3 (Netflix) expects **netflix_titles.csv** in `datasets/` — add the file if your notebook fails to load it. Project 8 (Mini Mart) uses synthetic data in the notebook. Project 11 (House Price) loads Boston Housing via OpenML. **Projects 12 and 17** load Titanic via Seaborn (`sns.load_dataset('titanic')`); **Project 18** (`GridSearchCV.ipynb` and `EnsembleLearning.ipynb`) loads Iris via Seaborn (`sns.load_dataset('iris')`); no CSV in `datasets/` is required for those notebooks.*

---

## Usage

- Run notebook cells top to bottom for full analysis.
- Adjust file paths if you move the repository or datasets.
- Use the same Python environment for consistent package versions.
- **Project 16:** Run `Fitness_tracker_ecommerce.ipynb` first if you need to regenerate `final_watch_data.csv`; then open `Model_creation.ipynb` (expects that CSV in the same folder).
- **Project 20:** Ensure `datasets/diabetes.csv` exists; after running `Diabetese_prediction.ipynb`, model artifacts are written under **`Project20 ML Diabetes Predictions/models/`** (create the folder if the notebook expects it and errors).

---

## License

This project is for educational and portfolio use.
