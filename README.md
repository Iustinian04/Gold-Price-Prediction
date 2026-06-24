# XAUUSD Algorithmic Trading Simulator

This repository contains a comprehensive trading framework for the **XAUUSD (Gold)** currency pair. The project explores the predictive capabilities of various Machine Learning and Deep Learning models to generate automated trading signals while incorporating risk management.

## Project Overview
The core objective of this project was to compare different architectural approaches in financial time-series forecasting. We evaluated how traditional tree-based models and recurrent neural networks perform when tasked with predicting short-term gold price movements in a volatile market environment.

## Frameworks & Technologies
The project relies on a robust stack for data engineering, model training, and backtesting:

* **Data Processing:** `pandas`, `numpy` for OHLCV data manipulation and technical indicator engineering.
* **Machine Learning:** `scikit-learn` for **Random Forest** implementation and `XGBoost` for gradient boosting regression.
* **Deep Learning:** `TensorFlow/Keras` for building and training **LSTM** (Long Short-Term Memory) networks.
* **Backtesting & Visualization:** `Streamlit` for the interactive dashboard and `Plotly` for high-fidelity trading chart visualizations.

## Key Features
* **Feature Engineering:** Includes EMA 200, ATR (Volatility), Bollinger Bands, VIX (Market Sentiment), and SMI (Stochastic Momentum Index).
* **Threshold Calibration:** A custom calibration mechanism to filter out market noise and trade only high-conviction signals, stabilizing the Win Rate.
* **Risk Management:** Integrated Stop-Loss (-0.10%) and Take-Profit (+0.30%) logic with a fixed 1:3 Risk/Reward Ratio.
* **Comparative Analysis:** Side-by-side performance metrics (Win Rate, Total Trades, Strategy Return vs. Market Baseline) for LSTM, Random Forest, and XGBoost.
