# Project 2 — Shopping Behaviour Analysis

## Problem Statement

Explore customer shopping behaviour data to understand purchasing patterns, preferences (category, size, color, season), payment methods, and how factors like discounts, subscription status, and review ratings influence buying behaviour. Insights can support marketing and inventory decisions.

## Dataset

- **Source:** `../datasets/shopping_trends.csv`
- **Key columns:** Customer ID, Age, Gender, Item Purchased, Category, Purchase Amount (USD), Location, Size, Color, Season, Review Rating, Subscription Status, Payment Method, Shipping Type, Discount Applied, Promo Code Used, Previous Purchases, Preferred Payment Method, Frequency of Purchases

## Analysis Performed

- **Understand dataset** — Load and explore transaction-level shopping data
- **Shape & info** — Data dimensions and column types
- **Missing values** — Identify and handle nulls
- **Target variable** — Purchase amount or frequency as outcome of interest
- **Categorical features** — Category, location, size, color, season, payment method, subscription status
- **Numerical features** — Age, purchase amount, review rating, previous purchases
- **Feature engineering** — Aggregations or segments (e.g. by category or location)
- **Correlation analysis** — Relationships among numerical variables
- **Visualization** — Countplots, boxplots, bar charts, heatmaps
- **Insights** — Key patterns and recommendations

## Key Insights (Summary)

- Most popular categories, items, and demographics
- Effect of discounts and promo codes on purchase behaviour
- Payment and shipping preferences by segment
- Relationship between review ratings and purchase patterns

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
