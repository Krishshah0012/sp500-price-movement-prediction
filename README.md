S&P 500 Price Movement Prediction

This project uses historical stock market data to predict S&P 500 index price movements using machine learning. By applying time-series feature engineering and a walk-forward validation approach, the model simulates realistic trading conditions to evaluate predictive performance.

Objective

The goal is to forecast short-term price direction (up or down) of the S&P 500 using past trends — helping simulate how algorithmic trading strategies might perform over time.

Features Engineered

- Rolling statistics (mean, standard deviation, min, max over 5/10/20-day windows)
- Price momentum and percentage returns
- Lagged returns and shifted values
- Target variable based on forward return (1 if market goes up, 0 otherwise)

Modeling and Evaluation

- Random Forest Classifier
- Walk-forward backtesting (simulates real trading by training on past and testing on future)
- Avoids data leakage and mimics realistic model deployment

Tools and Technologies

- Python, pandas, scikit-learn, matplotlib
- yfinance (for real-time stock market data)
- Jupyter Notebook

Results

- Achieved approximately 57% precision in out-of-sample predictions
- Demonstrated consistent performance across multiple market windows
- Outperformed random guessing and naive benchmarks
