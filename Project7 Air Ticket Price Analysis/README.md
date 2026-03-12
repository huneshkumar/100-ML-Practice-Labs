# Project 7 — Air Ticket Price Analysis

## Problem Statement

Analyze airline ticket pricing data to understand how factors such as airline, origin, destination, distance, travel class, and days before departure influence ticket prices. The goal is to identify pricing patterns and main drivers of price (e.g. distance, class, booking lead time).

## Dataset

- **Source:** `../datasets/airline_ticket_prices_dataset.csv`
- **Key columns:** Ticket_ID, Airline, Origin, Destination, Distance_km, Class, Days_Before_Departure, Price_USD (target)

## Analysis Performed

- **Understand dataset** — Load and explore ticket and route information
- **Shape & info** — Dimensions and data types
- **Missing values** — Check for nulls
- **Target variable** — Distribution of Price_USD; summary statistics
- **Categorical features** — Airline, Origin, Destination, Class (counts and price by segment)
- **Numerical features** — Distance_km, Days_Before_Departure, Price_USD
- **Feature engineering** — Route (origin–destination), price per km, or time buckets if used
- **Correlation analysis** — Correlation of distance and days before departure with price; heatmap
- **Visualization** — Histograms, boxplots (Class vs price, Airline vs price), scatter plots, heatmaps
- **Insights** — Main drivers of price and practical takeaways

## Key Insights (Summary)

- Effect of travel class (Economy, Business, First) on price
- Relationship between distance and ticket price
- Impact of days before departure on price (early vs late booking)
- Price variation by airline and popular routes

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
