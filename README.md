# Stock Price Forecasting — LSTM

[![Kaggle](https://img.shields.io/badge/Kaggle-View%20Notebook-20BEFF?logo=kaggle)]()

Predicts Apple stock closing prices using a stacked LSTM neural network 
trained on 6 years of historical data.

## Approach
- Downloaded AAPL historical data via yfinance (2018–2024)
- 60-day sliding window sequences as input features
- Stacked 2-layer LSTM with Dropout regularization
- Early stopping to prevent overfitting
- Evaluated on 20% held-out test set

## Results
- MAE and RMSE reported in USD on actual price scale
- Predicted vs Actual price chart shows strong trend-following behavior

![Forecast Results](lstm_stock_forecast.png)

## Tech Stack
Python · TensorFlow/Keras · yfinance · Pandas · NumPy · Scikit-learn

## Run It
Open in Kaggle or Colab. Install dependency: `pip install yfinance`
