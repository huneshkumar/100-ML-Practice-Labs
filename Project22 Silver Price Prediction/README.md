# Project 22 — Silver price forecast (EDA)

## Problem statement

Explore **forecast-style** silver price data: predicted levels, uncertainty bands, and time-based patterns (calendar features, volatility, rolling averages) to understand how the series behaves before building a dedicated forecasting model.

## Notebook

- **`notebooks/silver-price-forcast-EDA.ipynb`** — reads **`../dataset/silver_price_forecast_2026.csv`** (open the notebook from the **`notebooks/`** folder so relative paths work). Uses columns such as **Date**, **Predicted_Price**, **Lower_Bound**, **Upper_Bound**; adds or plots **day_of_week**, **volatility**, **rolling_mean_7**, etc. **`after-eda.csv`** is an optional exported stage in **`dataset/`**.

## Data

| File | Location |
|------|----------|
| `silver_price_forecast_2026.csv` | `Project22 Silver Price Prediction/dataset/` |
| `after-eda.csv` | same `dataset/` folder |

## Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
