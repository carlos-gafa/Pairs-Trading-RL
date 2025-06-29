##  Project Overview

This work explores the application of an **online actor-critic reinforcement learning (RL) agent**—enhanced with **LSTM networks**—to dynamically determine entry and exit points in a **pairs trading strategy**. The agent is tested across **daily and intraday (hourly)** financial data, incorporating realistic market constraints such as **transaction costs** and structural breaks.

Key contributions:
- A custom **LSTM-based online RL agent** trained with a replay buffer.
- Analysis across both **low- and high-frequency** trading regimes.
- Detailed performance comparison with:
  - Buy-and-hold strategies
  - Fixed-threshold pairs trading
  - Random baselines
- Implementation of statistical evaluation using **Sharpe Ratio** and **Kolmogorov–Smirnov tests**.

## Methodology Highlights

- Actor-Critic RL framework with LSTM for time series encoding
- Training with experience replay and hard target updates
- Feature inputs include **spread Z-score**, and technical indicators (e.g., RSI, MACD, OBV)
- Evaluation under multiple scenarios: with/without transaction costs

## 📊 Results Summary

- Best performance observed in **daily trading** scenarios with low transaction costs.
- RL agent outperformed traditional fixed-threshold models and random baselines.
- Model collapse under some settings prompted proposals for entropy-based exploration and stop-loss mechanisms in future work.


