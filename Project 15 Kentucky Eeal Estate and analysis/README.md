# Project 15 — Kentucky Real Estate EDA

## Problem Statement

Explore Kentucky real estate listing data to understand property types, list prices, square footage, beds, baths, garage capacity, year built, and how listing text relates to price. The goal is to summarize the market and identify patterns in home features and pricing.

## Dataset

- **Source:** `../datasets/kentucky_real_estate.csv`
- **Key columns:** type, sub_type, text (listing description), listPrice, sqft, stories, beds, baths, baths_full, baths_full_calc, garage, year_built

## Analysis Performed

- Load and inspect data; shape, info, missing values.
- Analyze categorical features (property type, sub_type).
- Analyze numerical features (price, sqft, beds, baths, year built).
- Correlation and visualizations (distributions, relationships).
- Document insights on the Kentucky housing listings sample.

## Key Insights (Summary)

- Price distribution and typical feature ranges for single-family and other types.
- Relationship between sqft, beds, baths, and list price.
- Data quality notes (missing sub_type, text fields).

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
