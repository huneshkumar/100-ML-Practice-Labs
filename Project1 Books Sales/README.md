# Project 1 — Books Sales Analysis

## Problem Statement

Analyze book sales data to understand which books, authors, genres, and publishers perform best in terms of sales, ratings, and revenue. The goal is to uncover patterns that can inform publishing and marketing decisions.

## Dataset

- **Source:** `../datasets/Books_Data_Clean.csv`
- **Key columns:** Publishing Year, Book Name, Author, language_code, Author_Rating, Book_average_rating, Book_ratings_count, genre, gross sales, publisher revenue, sale price, sales rank, Publisher, units sold

## Analysis Performed

- **Understand dataset** — Load and inspect book catalog with sales and rating metrics
- **Shape & info** — Dimensions, dtypes, and column overview
- **Missing values** — Check and handle nulls
- **Target/outcome** — Focus on gross sales, units sold, or sales rank as performance indicators
- **Categorical features** — Genre, author rating, language, publisher
- **Numerical features** — Ratings, ratings count, sale price, revenue, units sold
- **Feature engineering** — Derived metrics if needed (e.g. revenue per unit)
- **Correlation analysis** — Relationships between numerical variables
- **Visualization** — Histograms, bar charts, boxplots, scatter plots, heatmaps
- **Insights** — Summary of findings and recommendations

## Key Insights (Summary)

- Top-performing genres and publishers by sales and revenue
- Relationship between book ratings and sales/units sold
- Impact of author rating and sale price on performance
- Distribution of content by language and publishing year

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
