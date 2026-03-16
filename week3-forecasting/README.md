# Week 3 - Electricity Price Forecasting Pipeline

Time series forecasting model for hourly electricity prices built 
with Python, pandas and scikit-learn.

## What this project does
- Lag feature engineering (1hr, 24hr, 48hr, 168hr price history)
- Sequential train/test split (train 2015-2018 Q1, test 2018 Q2-Q4)
- Linear regression forecasting model with 8 input features
- Feature importance analysis
- Residual distribution analysis
- Hourly MAE breakdown identifying model weaknesses
- Model comparison: Week 1 MAE 9.48 → Week 3 MAE 1.95 EUR/MWh (79% improvement)

## Key Results
- MAE: 1.95 EUR/MWh (3.4% error rate)
- Identified price autocorrelation as dominant price driver
- lag1 coefficient: 0.8050 — previous hour price explains 80% of next hour price

## Dataset
Hourly Spanish electricity market data 2015-2018 (35,000+ observations)

## Tools
Python, pandas, matplotlib, scikit-learn
