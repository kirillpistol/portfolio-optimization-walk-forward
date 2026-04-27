# Portfolio Optimization with Walk-Forward Backtesting

## Overview

This project implements a realistic portfolio optimization framework designed to evaluate whether portfolio optimization adds value compared to simple allocation strategies under real-world conditions.

The model incorporates transaction costs, allocation constraints, and walk-forward validation to reduce overfitting and simulate practical investment scenarios.

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

## Results Overview

### Strategy Performance
![Strategy Comparison](strategy_comparison.png)

### Drawdowns
![Drawdowns](drawdowns.png)

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

## Key Results

- The optimized portfolio was compared against Equal Weight, Minimum Variance, and Risk Parity strategies
- Performance was evaluated out-of-sample using walk-forward backtesting
- Transaction costs (0.1%) were included in all strategies

  Key observation:

> Optimization does not always outperform simple strategies once transaction costs and constraints are applied.


## Why This Matters

In real-world portfolio management:

- Many optimized strategies fail due to overfitting  
- Transaction costs significantly reduce theoretical performance  
- Simple allocation strategies often outperform complex models  

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
This project demonstrates how to properly evaluate investment strategies using realistic assumptions.
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

## Strategies Implemented

- Optimized Portfolio (Max Sharpe Ratio)
- Equal Weight Portfolio
- Minimum Variance Portfolio
- Risk Parity Portfolio
- S&P 500 Benchmark

## Methodology

- Training window: 3 years (rolling)
- Test period: 2022–2024
- Rebalancing: Quarterly
- Optimization method: SLSQP
- Data source: Yahoo Finance (adjusted prices)

## Outputs

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\
The project generates:
\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

- Performance metrics (return, volatility, Sharpe ratio, drawdown)
- Portfolio weight evolution over time
- Rebalancing events and turnover
- Strategy comparison charts

## Tools

- Python
- Pandas / NumPy
- SciPy
- Matplotlib
- yFinance

## Project Structure

portfolio_walk_forward_backtest.ipynb
strategy_performance_raw.csv
all_weights_history.csv
all_rebalance_events.csv

## Author

Pistol Kirill
- SciPy
- yFinance
