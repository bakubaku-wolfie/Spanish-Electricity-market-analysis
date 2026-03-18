# Spanish Electricity Market Analysis

Python-based computational energy analysis portfolio built over 4 weeks.

## Projects

### Week 1 - Price Analysis Pipeline
Data loading, statistical analysis, correlation analysis and linear 
regression forecasting model.
- MAE: 9.48 EUR/MWh (baseline model)

### Week 2 - Market Dashboard
Multi-panel visualization dashboard covering intraday patterns, 
seasonal trends, generation mix correlation, price spike profiling 
and price duration curve.

### Week 3 - Forecasting Pipeline
Lag feature engineering, sequential validation and rolling 
walk-forward validation across 37 monthly windows.
- MAE improved from 9.48 → 1.95 EUR/MWh (79% improvement)
- Rolling average MAE: 2.27 EUR/MWh across all market conditions
- Identified seasonal model degradation: winter 3.4 vs summer 1.3 EUR/MWh

### Week 4 - Battery Arbitrage Optimization (coming soon)
Linear optimization model for battery charge/discharge scheduling 
to maximize profit from electricity price spreads.

## Tools
Python, pandas, matplotlib, seaborn, scikit-learn, statsmodels, numpy

## Dataset
Hourly Spanish electricity market data 2015-2018 (35,000+ observations)
