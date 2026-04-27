Walk-forward portfolio optimization with transaction costs, constraints and benchmark comparison
# Portfolio Optimization with Walk-Forward Backtesting

## Overview

This project implements a realistic portfolio optimization framework using:

- Walk-forward backtesting
- Transaction cost modeling (0.1%)
- Allocation constraints (max 40% per asset)
- Shrinkage regularization
- Benchmark comparison

## Strategies

- Optimized portfolio (Max Sharpe)
- Equal Weight
- Minimum Variance
- Risk Parity
- S&P 500 benchmark

## Methodology

- Training window: 3 years
- Rebalancing: Quarterly
- Optimization: SLSQP
- Out-of-sample evaluation

## Key Results

The model compares multiple strategies and evaluates whether optimization adds value over simple allocation methods.

## Output

- Performance metrics (return, volatility, Sharpe, drawdown)
- Portfolio weights over time
- Rebalancing events
- Strategy comparison charts

## Key Insight

Optimization only matters if it consistently outperforms simple benchmarks after transaction costs.

## Tools

- Python
- Pandas / NumPy
- SciPy
- yFinance
