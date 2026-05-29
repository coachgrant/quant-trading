# Quant Trading Research Scripts

This repository contains a collection of Python scripts I have been using to learn, test, and document quantitative trading concepts. The code covers market data collection, technical indicators, risk metrics, basic strategy logic, fundamental screening, and broker API practice.

The goal of this repository is not to present one finished trading system. It is a working research folder that shows the tools and ideas I have been building while studying quantitative finance and algorithmic trading.

## What this project does

This code is focused on four main areas:

1. Market data collection  
   Several scripts pull historical market data using sources such as Yahoo Finance. Other scripts connect to broker/demo APIs such as OANDA or FXCM for practice with live pricing, account data, candles, and order placement.

2. Technical indicator research  
   The project includes scripts that calculate common trading indicators such as:

   - RSI
   - MACD
   - ATR
   - ADX
   - Renko bricks
   - Volatility
   - Slope/momentum-style calculations

3. Strategy and signal testing  
   Some scripts test basic rule-based trading ideas, especially for forex pairs. Examples include RSI-based analysis, MACD/Renko logic, breakout-style logic, and simple long/short signal generation.

4. Performance and risk measurement  
   The repository includes scripts for measuring strategy or asset performance, including:

   - CAGR
   - Sharpe ratio
   - Sortino ratio
   - Maximum drawdown
   - Calmar ratio
   - Portfolio rebalancing concepts

There are also fundamental screening examples, including Piotroski F-score and Magic Formula-style stock ranking.

## What the code outputs

Depending on the script, the output may include:

- Downloaded OHLCV market data stored in pandas DataFrames
- Calculated technical indicator columns such as RSI, MACD, ATR, ADX, and Renko bar counts
- Printed performance metrics such as CAGR, drawdown, Sharpe ratio, Sortino ratio, and Calmar ratio
- Ranked stock lists from fundamental screening models
- Live/demo broker information such as bid/ask prices, account summaries, open trades, or order responses
- Trading signal messages such as buy, sell, close, or position update notifications

## Example workflow

A typical workflow in these scripts is:

1. Import market data
2. Clean missing values
3. Calculate indicators
4. Generate simple trading signals
5. Evaluate performance or risk
6. Print results or rankings for review

## Main files

| File | Purpose |
|---|---|
| `rsi.py` | Downloads forex data and calculates RSI values |
| `macd.py` | Calculates MACD and signal line logic |
| `adx.py` | Calculates ATR and ADX trend-strength indicators |
| `atr (1).py` | Calculates Average True Range for volatility/risk measurement |
| `renko.py` | Builds Renko-style price movement logic |
| `fx_macd_renko (8).py` | Combines forex data, MACD, Renko bricks, and trading signal logic |
| `cagr.py` | Calculates compound annual growth rate |
| `sharpe_sortino (1).py` | Calculates risk-adjusted return metrics |
| `max_dd_calmar (2).py` | Calculates maximum drawdown and Calmar ratio |
| `portfolio_rebalance (5).py` | Demonstrates portfolio rebalancing logic |
| `piotroski_f.py` | Screens stocks using Piotroski F-score concepts |
| `magic_formula (1).py` | Screens stocks using Magic Formula-style value metrics |
| `oanda (11).py` | Demonstrates OANDA practice API connection, pricing, candles, account data, and order placement |

## Notes

This is a learning and research repository. Some scripts are standalone examples and may need API keys, package installation, or updated data sources before running. Broker-related scripts are intended for practice/demo environments unless reviewed and modified carefully.

The next improvement for this repository is to organize the scripts into folders, clean up file names, add requirements, and separate research scripts from broker execution scripts.

## Disclaimer

This code is for educational and research purposes only. It is not financial advice and should not be used for live trading without further testing, risk controls, and review.
