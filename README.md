# Equity Screening System — Stage 1 Universe Filter

**Tools:** Thinkorswim, TradingView  
**Indicators:** Moving Averages (200/50-day), RSI, ADX, EPS, Volume, Market Cap, Range Filter

---

## Overview

This repository documents a multi-stage equity screening framework built in Thinkorswim. 
The system filters the broad equity universe down to a focused candidate list using 
momentum, trend strength, and liquidity criteria — before deeper technical analysis is applied.

---

## Stage 1: Universe Screener

The first-pass filter eliminates illiquid, unprofitable, and weak-trend stocks from consideration.

| Filter                     | Threshold     | Purpose                                      |
|----------------------------|---------------|----------------------------------------------|
| 200-Day MA Strength        | ≥ 7.5%        | Confirms long-term uptrend                   |
| 50-Day MA Strength         | ≥ 5%          | Confirms intermediate trend momentum         |
| RSI (14)                   | > 25          | Excludes deeply oversold / broken stocks     |
| ADX (14)                   | Breakout only | Filters for directional strength             |
| Range Filter               | 75            | Targets stocks with sufficient price action  |
| Market Cap                 | ≥ $300M       | Ensures institutional liquidity              |
| EPS (TTM)                  | > 0           | Excludes unprofitable companies              |
| Average Volume             | ≥ 500K shares | Eliminates thinly traded securities          |

---

## Roadmap

- [ ] Stage 2: Momentum setup identification within filtered universe  
- [ ] Breakout timing and entry signal development  
- [ ] Python replication of screening logic  
- [ ] Backtesting and strategy performance evaluation
