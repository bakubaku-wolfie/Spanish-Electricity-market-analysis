# Week 3 - Electricity Price Forecasting Pipeline

Time series forecasting model for hourly electricity prices built 
with Python, pandas and scikit-learn.

## File 1: week3_forecasting_pipeline.ipynb
Full forecasting model with all features and sequential validation.

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

## File 2: week3_rolling_validation.ipynb
Walk-forward validation testing model robustness across time.

### What it does
- Monthly walk-forward validation across 37 time windows
- Tests model performance across different market conditions
- Monthly MAE bar chart visualization

### Key Results
- Average rolling MAE: 2.27 EUR/MWh | Std deviation: 0.65 EUR/MWh
- Winter degradation: MAE peaks at 3.4 EUR/MWh (Jan/Mar)
- Summer performance: MAE as low as 1.3 EUR/MWh (Jun/Jul)
- Model reliable in stable markets, stressed in volatile winters

## Dataset
Hourly Spanish electricity market data 2015-2018 (35,000+ observations)

## Tools
Python, pandas, matplotlib, scikit-learn, statsmodels, numpy
