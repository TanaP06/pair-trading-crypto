# Pair Trading Strategy using Cointegration

This project implements a **statistical arbitrage (pair trading) strategy** based on
cointegration testing and z-score signals.

The system identifies cointegrated asset pairs, constructs a mean-reverting price
ratio, and executes a rule-based trading strategy to evaluate performance.

---

## Project Objectives

- Identify statistically cointegrated asset pairs
- Construct a mean-reverting trading signal
- Backtest a pair trading strategy
- Evaluate performance using Sharpe ratio

---

## Methodology

1. **Data Collection**
   - Historical daily price data
   - Assets filtered for missing values

2. **Data Preprocessing**
   - Cleaning and normalization
   - Train / validation / test split

3. **Pair Selection**
   - P-value threshold to select valid pairs

4. **Signal Construction**
   - Price ratio between two assets
   - Rolling z-score based on long and short windows

5. **Trading Strategy**
   - Enter long/short positions when z-score exceeds thresholds
   - Exit positions when z-score reverts toward zero

6. **Performance Evaluation**
   - Sharpe ratio

---

## Tech Stack

- Python 3
- NumPy
- Pandas
- SciPy
- Statsmodels
- Scikit-learn
- Matplotlib
