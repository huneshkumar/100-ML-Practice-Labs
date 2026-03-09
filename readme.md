# EDA Projects

A collection of **Exploratory Data Analysis (EDA)** projects demonstrating data cleaning, visualization, and insight extraction using Python, Pandas, and visualization libraries.

---

## Overview

This repository contains hands-on EDA projects built with Jupyter notebooks. Each project focuses on real-world datasets and covers data loading, quality checks, visualization, and actionable insights.

---

## Projects

| Project | Description | Dataset |
|--------|-------------|---------|
| **Project 1 — Books Sales** | Analysis of book sales, ratings, genres, and publisher performance. | `Books_Data_Clean.csv` |
| **Project 2 — Shopping Behaviour** | Exploration of customer shopping trends and purchasing patterns. | `shopping_trends.csv` |
| **Project 3 — Netflix Movies & TV Shows** | Analysis of Netflix content distribution, genres, and growth over time. | Netflix dataset |

---

## Repository Structure

```
.
├── datasets/
│   ├── Books_Data_Clean.csv
│   └── shopping_trends.csv
├── Project1 Books Sales/
│   └── Books.ipynb
├── Project2 Shopping Behavioure/
│   └── customerShoppingBehavioure.ipynb
├── Project3 Netflix Movies & TV Shows Analysis/
│   └── NetflixAnalysis.ipynb
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

Netflix project may use a separate dataset; refer to the notebook for source and path.

---

## Usage

- Run notebook cells top to bottom for full analysis.
- Adjust file paths if you move the repository or datasets.
- Use the same Python environment for consistent package versions.

---

## License

This project is for educational and portfolio use.
