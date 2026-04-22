---
title: "Vol-Smile Arbitrage"
excerpt: "SPY volatility arbitrage on 4yr EOD NBBO option chains. Combined OOS Sharpe 0.78, FF5+UMD+ΔVIX+VRP alpha t=2.68.<br/>[GitHub](https://github.com/lexilei/vol_smile)"
collection: portfolio
published: false
---

SPY volatility arbitrage backtest over four years of ThetaData EOD NBBO option chains. I fit per-expiry SVI smiles, compute Black–Scholes IVs, and use an EWMA z-score on moneyness-bucket residuals to flag rich/cheap options. Positions are delta-hedged daily with a VIX regime filter.

Walk-forward evaluation uses 39 windows (IS=126d, OOS=63d, 5d purge). Combined OOS Sharpe is **0.78**, and a FF5 + UMD + ΔVIX + VRP factor regression gives alpha **t = 2.68** (p = 0.008) with a residual Sharpe of **1.41**. Generalized to QQQ (SPY return correlation −0.007, vol-targeted Sharpe 1.23), the combined two-asset portfolio Sharpe is **1.36**.

The full-sample Sharpe of 1.11 is overfit — 0.78 is the honest out-of-sample number.

[Code](https://github.com/lexilei/vol_smile)
