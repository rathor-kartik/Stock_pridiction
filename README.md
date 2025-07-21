# 📈 AAPL Stock Price Prediction using LSTM

This project demonstrates how to use a Long Short-Term Memory (LSTM) neural network for time series forecasting of **Apple Inc. (AAPL)** stock closing prices using historical data from Yahoo Finance.

---

## 🔍 Project Overview

- **Data Source:** Yahoo Finance via `yfinance`
- **Model:** LSTM (Long Short-Term Memory) using TensorFlow/Keras
- **Data Range:** 2015-01-01 to 2024-12-31
- **Goal:** Predict the next closing price using the past 60 days of closing prices

---

## 🧰 Libraries Used

- `numpy`
- `pandas`
- `matplotlib`
- `yfinance`
- `scikit-learn`
- `tensorflow` / `keras`

---

## 🚀 How It Works

1. **Fetch Data:** Downloads historical AAPL stock prices (Close only).
2. **Preprocessing:**
   - Scales the data to range [0,1]
   - Creates time series sequences
3. **Build LSTM Model:**
   - 2 stacked LSTM layers + 1 Dense output layer
   - Trained with MSE loss
4. **Evaluate:**
   - Predictions are inverse-transformed
   - Evaluated using RMSE (~6.32)
5. **Visualize:**
   - Plot actual vs. predicted closing prices

---

## 📊 Result

The model effectively tracks trends in AAPL closing prices. While not perfect, the predictions closely follow the actual stock behavior.


