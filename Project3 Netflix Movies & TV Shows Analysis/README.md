# Project 3 — Netflix Movies & TV Shows Analysis

## Problem Statement

Perform Exploratory Data Analysis on Netflix’s content catalog to understand content distribution, popular genres, the balance between movies and TV shows, and how the library has grown over time. Results support content strategy and user-facing recommendations.

## Dataset

- **Source:** `../datasets/netflix_titles.csv`
- **Key columns:** show_id, type, title, director, cast, country, date_added, release_year, rating, duration, listed_in (genres), description

## Analysis Performed

- **Understand dataset** — Load and explore Netflix title metadata
- **Shape & info** — Dimensions, dtypes, column overview
- **Missing values** — Check director, cast, country and other nulls
- **Target/focus** — Content type (Movie vs TV Show), release year, genres
- **Categorical features** — Type, rating, country, listed_in (genres)
- **Numerical/temporal** — release_year, date_added, duration (parsed)
- **Feature engineering** — Extract year from date_added, parse duration, expand genres
- **Correlation/patterns** — Trends over time, type vs genre
- **Visualization** — Countplots, bar charts, time series, heatmaps
- **Insights** — Summary of distribution and growth

## Key Insights (Summary)

- Proportion of movies vs TV shows and trends over time
- Most common genres and content ratings
- Geographic distribution (country) of content
- Content growth by year and by type

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
