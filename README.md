# Equity Screening Systems

## Overview
This repository contains equity screening models built using Thinkorswim to identify stocks based on momentum, trend strength, and liquidity filters.

The goal of this project is to develop a structured, multi-stage approach to equity analysis used to filter stocks and identify those with strong forward-looking potential.



## Purpose
The purpose of this project is to identify stocks with strong momentum, volume, and trend characteristics that may indicate continued directional movement, and to filter the broader equity universe into a focused set of candidates for further analysis.

---

## Stage 1: Universe Screener

This initial screening layer is used to identify stocks that meet specific liquidity, momentum, and trend-based criteria.

### Filters Used:
- 200-day moving average strength ≥ 7.5%
- 50-day moving average strength ≥ 5%
- RSI (14) > 25
- ADX (14) breakout filter
- Market cap ≥ $300M
- Volume ≥ 500K
- Range filter (75)

### Stage Objective
This screener serves as a first-pass market filter to eliminate illiquid and weak-trend stocks before deeper analysis is applied.



## Future Expansion
- Momentum-based trade setup identification
- Breakout timing and entry signal development
- Python-based replication of screening logic
- Backtesting and performance evaluation of strategies



## Tools Used
- Thinkorswim (TOS): Used for building and running custom equity screeners, applying technical filters, and scanning large stock universes.
- TradingView: Chart analysis and technical validation of screened stocks
- Technical indicators (MA, RSI, ADX): Used to define trend, momentum, and strength conditions
