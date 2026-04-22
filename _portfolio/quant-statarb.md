---
title: "Quant StatArb: Kalman-Filter Pairs Trading"
excerpt: "Cointegration-based pairs trading with Kalman-filter dynamic hedge ratios under sector/beta neutrality.<br/>[GitHub](https://github.com/lexilei/quant-statarb-kalman)"
collection: portfolio
---

Statistical arbitrage on cointegrated equity pairs. Pairs are selected by Engle–Granger cointegration tests with an AR(1) half-life filter on the spread, and hedge ratios are updated online via a Kalman filter with recursive Bayesian updates so that the hedge tracks regime drift instead of assuming a constant beta.

Backtested walk-forward under sector- and beta-neutrality constraints.

[Code](https://github.com/lexilei/quant-statarb-kalman)
