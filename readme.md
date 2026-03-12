# EDA Projects

A collection of **Exploratory Data Analysis (EDA)** projects demonstrating data cleaning, visualization, and insight extraction using Python, Pandas, and visualization libraries.

---

## Overview

This repository contains hands-on EDA projects built with Jupyter notebooks. Each project focuses on real-world datasets and covers data loading, quality checks, visualization, and actionable insights.

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
| **Project 3 — Netflix Movies & TV Shows** | Analysis of Netflix content distribution, genres, and growth over time. | `netflix_titles.csv` |
| **Project 4 — Medical Insurance Cost** | Analysis of medical insurance costs and factors affecting premiums. | `insurance.csv` |
| **Project 5 — Heart Disease Analysis** | EDA of heart disease indicators and related health metrics. | `heart.csv` |
| **Project 6 — Titanic Data Analysis** | Analysis of Titanic passenger data and survival patterns. | `titanic.csv` |
| **Project 7 — Air Ticket Price Analysis** | Analysis of airline ticket prices and pricing factors. | `airline_ticket_prices_dataset.csv` |
| **Project 8 — Mini Mart Customer Analysis** | Analysis of mini mart customer behavior and purchasing patterns. | See notebook |

Each project folder contains a **README.md** with problem statement, dataset details, analysis steps, and key insights.

---

## Repository Structure

```
.
├── datasets/
│   ├── Books_Data_Clean.csv
│   ├── shopping_trends.csv
│   ├── netflix_titles.csv
│   ├── insurance.csv
│   ├── heart.csv
│   ├── titanic.csv
│   └── airline_ticket_prices_dataset.csv
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
   pip install pandas numpy matplotlib seaborn jupyter
   ```

4. **Launch Jupyter**:

   ```bash
   jupyter notebook
   ```

5. Open any `.ipynb` file from the project folders. Ensure notebook paths point to the `datasets/` folder when loading CSVs.

---

## Datasets

- **Books_Data_Clean.csv** — Book metadata, ratings, sales, and publisher information.
- **shopping_trends.csv** — Customer shopping and trend data for behaviour analysis.
- **netflix_titles.csv** — Netflix movies and TV shows catalog for content analysis.
- **insurance.csv** — Medical insurance cost data for cost and premium analysis.
- **heart.csv** — Heart disease and cardiovascular health indicators for analysis.
- **titanic.csv** — Titanic passenger and survival data for demographic and outcome analysis.
- **airline_ticket_prices_dataset.csv** — Airline ticket pricing data for price and factor analysis.

---

## Usage

- Run notebook cells top to bottom for full analysis.
- Adjust file paths if you move the repository or datasets.
- Use the same Python environment for consistent package versions.

---

## License

This project is for educational and portfolio use.
