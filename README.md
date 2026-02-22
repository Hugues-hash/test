# Detecting distribution shift in financial time series

## Problem
Financial time series are non-stationary: their statistical properties change over time. Models trained on historical data may degrade when the underlying distribution shifts.

This project investigates:
- whether distribution shift can be detected using statistical methods
- how predictive model performance evolves under drift
- whether drift signals correlate with performance degradation

The focus is on monitoring and robustness, not prediction accuracy.

## Movitvation
In deployed ML systems, especially in finance, model stability is critical. Even simple models may fail silently when input distributions change.

This project simulates a simple monitoring system that:
- detect feature distribution changes
- tracks model performance over time
- highlights periods of instability

## Dataset
- Asset: (e.g., S&P 500 ETF – SPY)
- Frequency: Daily
- Period: e.g., 2005–2024
- Source: Yahoo Finance (public data)
### Features:
- Returns
- Rolling mean
- Rolling volatility
- Lagged returns

### Target: Next-day return value (regression)

