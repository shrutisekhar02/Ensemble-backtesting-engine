#  LSTM and Bollinger Bands Stock Backtesting Engine

This project implements a hybrid stock trading strategy that combines deep learning and technical analysis. An LSTM model is trained to predict the next day’s stock price using a 50-day historical window. These forecasts are combined with Bollinger Band signals to generate high-confidence buy/sell decisions. The system is backtested across a portfolio of 50 large-cap stocks, evaluating both returns and risk metrics. Performance is visualized using QuantStats, and results demonstrate strong alignment between model predictions and actual market movements

---

##  Content

- `Data/`  
  → Folder containing CSV price data for 50 large-cap stocks used in backtesting.

- `generate_signal.py`  
  → Contains the ensemble signal generation logic using LSTM predictions and Bollinger Bands.

- `lstm_12_p50_ckp_13_24_e150.h5`  
  → Pre-trained LSTM model that predicts the next day's stock price from the past 50 days.

- `LSTM_Stock_Price_Prediction.ipynb`  
  → Jupyter notebook used to train and evaluate the LSTM model.

- `Backtest.ipynb`  
  → Full pipeline notebook: loads data, registers the model, generates signals, and evaluates performance.

- `requirements.txt`  
  → Lists Python package dependencies required to run the project.

- `README.md`  
  → Documentation outlining the project, methodology, setup, and usage.
