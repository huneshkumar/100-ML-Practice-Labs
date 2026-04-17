# EDA Projects

A collection of **Exploratory Data Analysis (EDA)** and **Machine Learning (ML)** projects (regression, classification, clustering, and time-series style EDA) across **22** themed folders, demonstrating data cleaning, visualization, insight extraction, and prediction using Python, Pandas, and visualization libraries.

---

## Contents

- [Overview](#overview)
- [Data Science and ML Roadmap](#data-science-and-ml-roadmap)
- [EDA Checklist](#eda-checklist)
- [Chart Selection Guide](#chart-selection-guide)
- [Projects](#projects)
- [Repository Structure](#repository-structure)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Datasets](#datasets)
- [Usage](#usage)
- [License](#license)

---

## Overview

This repository contains hands-on EDA and ML projects built with Jupyter notebooks. EDA projects focus on real-world datasets with data loading, quality checks, visualization, and insights. Supervised ML projects (**9–12**, **15**–**20**) add regression or classification models, train/test evaluation, and metrics (e.g. R², accuracy). **Project 18** covers **hyperparameter search** (`GridSearchCV`, `RandomizedSearchCV` on Iris) and **`EnsembleLearning.ipynb`** (stacking, random forest, AdaBoost, gradient boosting, **XGBoost**). **Project 19** is **sonar** rock vs metal classification; **Project 20** is **diabetes** prediction with **SVM** + **`GridSearchCV`**. **Project 21** is **unsupervised learning**: **`make_blobs`**, **`StandardScaler`**, **elbow** / **KMeans**, and **DBSCAN**. **Project 22** is **silver price** exploratory work on a **project-local** forecast CSV (plots, rolling stats). Use the **[Data Science and ML Roadmap](#data-science-and-ml-roadmap)** as a step-by-step study guide from problem framing through deployment. Each project folder has its own **README.md** with problem statement, dataset description, analysis steps, and key insights.

---

## Data Science and ML Roadmap

End-to-end flow from framing a question to operating a model in the real world. Use it as a study order or checklist when building projects (many steps map to notebooks in this repo).

| Step | Phase | What to do |
|:----:|--------|------------|
| **1** | **Problem & success criteria** | Clarify the business or research question, define **success metrics** (e.g. RMSE, accuracy, precision/recall), constraints (latency, fairness, budget), and what “good enough” means. |
| **2** | **Data collection** | Gather data from files, databases, APIs, surveys, or sensors; document **provenance**, **licenses**, and **sampling**; version raw snapshots when possible. |
| **3** | **Exploratory Data Analysis (EDA)** | Inspect schema, **dtypes**, **shape**, **missing values**, duplicates, and **distributions**; visualize relationships; form hypotheses (see [EDA Checklist](#eda-checklist)). |
| **4** | **Cleaning & preprocessing** | Handle missingness and outliers; fix types; parse dates/categories; **normalize/standardize** when algorithms require it; avoid **data leakage** from future information. |
| **5** | **Feature engineering & selection** | Create ratios, bins, interactions; **encode** categoricals; drop or combine redundant columns; optional **feature selection** or dimensionality reduction. |
| **6** | **Experimental design** | Choose **train / validation / test** splits (or **cross-validation**); use **stratification** for imbalanced classification; set a **random seed** for reproducibility. |
| **7** | **Baseline model** | Train a **simple, interpretable** model first (e.g. linear or logistic regression) to establish a **reference score** and sanity-check the pipeline. |
| **8** | **Modeling & comparison** | Try stronger algorithms (trees, ensembles, SVMs, neural nets where appropriate); compare metrics on the **same validation protocol**. |
| **9** | **Hyperparameter tuning** | Improve models with **`GridSearchCV`**, **`RandomizedSearchCV`**, or other search methods; keep a **held-out test** set untouched until final reporting. |
| **10** | **Evaluation & error analysis** | Report **test** performance; study **residuals**, **confusion matrices**, calibration, and failure cases; check stability across folds or slices of data. |
| **11** | **Interpretability & storytelling** | Summarize **drivers** of predictions (coefficients, feature importance, partial dependence); turn results into **clear visuals and recommendations** for stakeholders. |
| **12** | **Deployment, monitoring, & iteration** | Package the model (**pickle** / **joblib** / MLflow, etc.), expose **batch or API** scoring, log predictions, watch for **data drift**, and plan **retraining** when performance drops. |

**Note:** Steps **1–6** are mostly data work; **7–10** are core ML; **11–12** connect ML to decisions and production. You can loop back to **3–9** whenever new data arrives or the problem definition changes.

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
| **Project 18 — Hyperparameter tuning & ensembles** | **Iris** (Seaborn): **`GridSearchCV.ipynb`** — **k-NN** and **SVC** baselines, **`GridSearchCV`** (5-fold CV) on SVM and k-NN, **`RandomizedSearchCV`** on SVM. **`EnsembleLearning.ipynb`** — **EDA** by **species**; **`LabelEncoder`** + **stratified** train/test split; **`StackingClassifier`** (DT + **SVC** `probability=True` + **LR** → logistic meta, `cv=5`); **`RandomForestClassifier`** (`n_estimators=100`, `max_depth=None`, `random_state=42`); **`#adaboost`** — **`AdaBoostClassifier`** (`n_estimators=100`), **`GradientBoostingClassifier`** (`n_estimators=100`, `learning_rate=0.1`), **`XGBClassifier`** (`n_estimators=100`, `learning_rate=0.1`, `max_depth=3`, `eval_metric='mlogloss'`); **`accuracy_score`** on test for each. | Seaborn `sns.load_dataset('iris')` |
| **Project 19 — Sonar: mine vs rock classification** | **Binary classification:** 60 sonar frequency-energy features plus label **R** (rock) vs **M** (metal); EDA, train/test split, **logistic regression**, train and test **accuracy**, and a worked **prediction** example (`Sonar_mine_prediction.ipynb`). | `sonar_data.csv` |
| **Project 20 — ML: Diabetes prediction** | **Binary classification (Pima-style):** load **`diabetes.csv`**, EDA (`Outcome` balance, group means), **`StandardScaler`** on features, train/test split, **`GridSearchCV`** over **SVC** (`C`, `kernel`), train/test **accuracy**, sample inference, **`joblib`** export of fitted model and scaler to **`models/`** (`Diabetese_prediction.ipynb`). | `diabetes.csv` |
| **Project 21 — Unsupervised learning (clustering)** | **`make_blobs`** synthetic 2D data; **`StandardScaler`**; **elbow** curve over **K**; **`KMeans`** (e.g. `n_clusters=3`); alternate **KMeans** / **`DBSCAN`** (`eps`, `min_samples`) with **Seaborn** scatterplots by cluster (`Clustring.ipynb`). | `sklearn.datasets.make_blobs` (synthetic) |
| **Project 22 — Silver price prediction (EDA)** | Load **`silver_price_forecast_2026.csv`** from the project **`dataset/`** folder; **EDA** and visuals on **Date**, **Predicted_Price**, bounds, **day_of_week**, **volatility**, rolling means (`notebooks/silver-price-forcast-EDA.ipynb`). | `Project22 Silver Price Prediction/dataset/silver_price_forecast_2026.csv` |

Each project folder contains a **README.md** with problem statement, dataset details, analysis steps, and key insights (**Projects 9–12 and 15–22** include modeling, tuning, evaluation, clustering, or EDA pipelines as listed above).

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
├── Project15 Kentucky Eeal Estate and analysis/
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
├── Project21 Unsupervised Learning/
│   ├── Clustring.ipynb
│   └── README.md
├── Project22 Silver Price Prediction/
│   ├── dataset/
│   │   ├── silver_price_forecast_2026.csv
│   │   └── after-eda.csv
│   ├── notebooks/
│   │   └── silver-price-forcast-EDA.ipynb
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
- **Scikit-learn** — for Projects 9–12 and **15**–**22** (linear/logistic regression, k-NN, naive Bayes, SVM, tree/ensemble models, **`StackingClassifier`**, **`RandomForestClassifier`**, **`AdaBoostClassifier`**, **`GradientBoostingClassifier`**, **`KMeans`**, **`DBSCAN`**, **`GridSearchCV`** / **`RandomizedSearchCV`**, **`make_blobs`**, train/test split, scaling, metrics, OpenML where used, classification/regression evaluation)
- **XGBoost** — optional for **Project 18** **`EnsembleLearning.ipynb`** (`XGBClassifier` on Iris; install if you run those cells)
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

   For **Project 18** (`EnsembleLearning.ipynb`, **XGBoost** section), also install:

   ```bash
   pip install xgboost
   ```

4. **Launch Jupyter**:

   ```bash
   jupyter notebook
   ```

5. Open any `.ipynb` file from the project folders. For CSV-based projects, ensure paths point to the `datasets/` folder when loading data (e.g. `../datasets/filename.csv` from a project folder).

**Folder naming:** Kentucky real estate lives under **`Project15 Kentucky Eeal Estate and analysis/`** (no space after `Project15`). If your local clone used a different spelling, match the folder name on disk when opening notebooks.

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
- **Silver price (Project 22)** — **`silver_price_forecast_2026.csv`** and **`after-eda.csv`** live under **`Project22 Silver Price Prediction/dataset/`** (not the shared root `datasets/` folder). The notebook loads them via **`../dataset/`** from **`notebooks/`**.

*Project 3 (Netflix) expects **netflix_titles.csv** in `datasets/` — add the file if your notebook fails to load it. Project 8 (Mini Mart) uses synthetic data in the notebook. Project 11 (House Price) loads Boston Housing via OpenML. **Projects 12 and 17** load Titanic via Seaborn (`sns.load_dataset('titanic')`); **Project 18** loads Iris via Seaborn (`sns.load_dataset('iris')`); **Project 21** uses **`sklearn.datasets.make_blobs`**. No CSV in the root **`datasets/`** folder is required for those. **`EnsembleLearning.ipynb`** also uses **XGBoost** (install separately; the notebook may include a `pip install xgboost` cell).*

---

## Usage

- Run notebook cells top to bottom for full analysis.
- Adjust file paths if you move the repository or datasets.
- Use the same Python environment for consistent package versions.
- **Project 3:** The Netflix notebook filename on disk may start with a **leading space** (` NetflixAnalysis.ipynb`). If it does not appear in Jupyter or your file tree, rename it to `NetflixAnalysis.ipynb` (no leading space).
- **Project 18:** Run **`EnsembleLearning.ipynb`** with **`xgboost`** installed for the **`XGBClassifier`** section (see **Getting Started**), or execute the notebook’s install cell first.
- **Project 16:** Run `Fitness_tracker_ecommerce.ipynb` first if you need to regenerate `final_watch_data.csv`; then open `Model_creation.ipynb` (expects that CSV in the same folder).
- **Project 20:** Ensure `datasets/diabetes.csv` exists; after running `Diabetese_prediction.ipynb`, model artifacts are written under **`Project20 ML Diabetes Predictions/models/`** (create the folder if the notebook expects it and errors).
- **Project 22:** Open **`silver-price-forcast-EDA.ipynb`** from **`Project22 Silver Price Prediction/notebooks/`** so the relative path **`../dataset/silver_price_forecast_2026.csv`** resolves correctly.

---

## License

This project is for educational and portfolio use.
