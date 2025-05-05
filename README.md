# Multi--Horizon-Stock-Price-Forecasting-using-ARIMA-XGBoost-and-LSTM.
This project predicts stock trends for top S&amp;P 500 companies using a hybrid ARIMA-XGBoost-LSTM model. It forecasts 1-day, 5-day, and 20-day movements using technical indicators and sentiment analysis. Outputs include confidence-based predictions and direction forecasts, evaluated using RMSE, MAE, and accuracy metrics for reliable market insights.

🚀 Key Features
Multi-Horizon Forecasting: Predicts short-term (1-day), medium-term (5-day), and long-term (20-day) stock prices.

Hybrid Modeling: Integrates ARIMA for linear trends, XGBoost for non-linear features, and LSTM for temporal dependencies.

Feature Engineering: Incorporates technical indicators like RSI, MACD, and EMA.

Sentiment Analysis: Future integration of financial news for context-aware predictions.

Evaluation Metrics: Uses RMSE, MAE, Directional Accuracy, Precision, and Recall.

Confidence Intervals: Provides probabilistic bounds for each forecast.

Visual Output: Plots predicted vs actual prices and directional trends.

🛠️ Technologies Used
Python

NumPy, Pandas

scikit-learn

statsmodels (ARIMA)

XGBoost

TensorFlow / Keras (LSTM)

TA-Lib or ta for technical indicators

Matplotlib & Seaborn for visualization

📊 Dataset
Source: Yahoo Finance & Alpha Vantage

Scope: Historical OHLCV data of top 100 S&P 500 stocks

Features: Price data + Technical indicators (EMA, RSI, MACD)

⚙️ Project Structure
kotlin
Copy
Edit
├── data/
│   └── raw & preprocessed stock data
├── models/
│   ├── arima_model.py
│   ├── xgboost_model.py
│   └── lstm_model.py
├── utils/
│   └── preprocessing.py, feature_engineering.py
├── notebooks/
│   └── analysis and visualization
├── results/
│   └── prediction_outputs/
│       ├── *_metrics.txt
│       └── *_predictions.txt
├── main.py
├── README.md
└── requirements.txt

🧪 Evaluation Results
Horizon	Avg RMSE	Avg MAE	Directional Accuracy
1-Day	19.27	13.69	48.7%
5-Day	21.09	15.50	48.7%
20-Day	26.11	19.81	49.3%

Example Prediction for Amazon:
1-day: $169.00 (CI: $135.59 - $202.41)
5-day: $168.00 (CI: $134.05 - $201.94)
20-day: $174.31 (CI: $138.49 - $210.13)


✅ Future Improvements
Implement XGBoost-LSTM hybrid modeling

Add real-time predictions via API

Apply k-fold/time series cross-validation

Integrate sentiment data from financial news

Explore Transformer-based models for long-term dependencies
