---
title: "Alpha-Graph: NLP-Driven Equity Signal Generation"
excerpt: "Signal pipeline over 4,146 8-K and 401 10-K SEC filings. Walk-forward LightGBM with HMM regime detection. Sharpe 1.91 OOS.<br/>[GitHub](https://github.com/lexilei/alpha-graph)"
collection: portfolio
published: false
---

NLP-driven equity signal over SEC filings. The corpus is 4,146 8-Ks and 401 10-Ks covering 102 S&P 500 tickers; I score 25 item types with exponential decay and TF-IDF cosine similarity against the firm's own annual filings to capture novelty.

Signals feed a walk-forward LightGBM model with a 12-month training window and a 5-day purge. An HMM regime filter and anti-momentum features shape sizing. Over an 18-month out-of-sample period: Sharpe **1.91**, cumulative return **+87.2%**, and critically bilateral alpha — the short leg earns a Sharpe of **+0.75** on its own.

[Code](https://github.com/lexilei/alpha-graph)
