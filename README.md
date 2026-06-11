# Nifty 50 Direction Predictor

A machine learning model that predicts whether 
Nifty 50 closes higher or lower the next trading day.

## Results
- Out-of-sample accuracy: 52.51%
- Outperforms Buy & Hold by ₹3,824 after realistic 
  transaction costs over 2 year test period
- Test period: 2024–2026

## Features Used
- S&P 500 previous day return
- India VIX (fear index)
- Bank Nifty / Nifty ratio
- Crude oil return
- Gold return  
- Rolling volatility (20-day)
- 50-day trend ratio
- Previous day return

## Model
- Algorithm: Random Forest Classifier
- Threshold: optimized using probability calibration
- Minimum holding period: 3 days
- Transaction costs modeled: ₹120 entry + 0.1% exit tax + ₹25 flat

## Tech Stack
- Python, scikit-learn, yfinance, pandas, matplotlib

## How to Run
pip install yfinance scikit-learn pandas matplotlib numpy
# Then open nifty_predictor.ipynb in Jupyter or Colab
