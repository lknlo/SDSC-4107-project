# SDSC 4107 Project: Financial Volatility and Risk Modeling
## Overview
This project implements a comprehensive pipeline for financial time series analysis, focusing on volatility prediction, tail risk modeling, and dynamic portfolio optimization using machine learning and deep learning techniques. The code is designed for research and educational purposes, leveraging S&P 500 data and interest rate forecasting.

## Features
- Data Acquisition: Downloads S&P 500 historical data using yfinance.
- Feature Engineering: Computes realized volatility, moving averages, lagged returns, and advanced tail risk features (skewness, kurtosis, VaR, ES, extreme events, correlations).
- Volatility Prediction: Implements Random Forest, Support Vector Machine (SVM), and Neural Network models to predict future realized volatility.
- Tail Risk Modeling: Builds a neural network to classify tail risk events using engineered features.
- Dynamic Portfolio Optimization: Adjusts portfolio weights based on predicted volatility and tail risk using quadratic programming ( cvxopt ).
- Interest Rate Forecasting: Uses deep learning (PyTorch) to predict future interest rates and visualize results.
- Visualization: Plots actual vs. predicted volatility, scatter plots for model evaluation, and interest rate forecasts.
## Requirements
- Python 3.7+
- pandas, numpy, matplotlib, yfinance
- scikit-learn, tensorflow, torch
- cvxopt
Install dependencies with:

```
pip install pandas numpy matplotlib 
yfinance scikit-learn tensorflow torch 
cvxopt
```
## Usage
1. Run the script:
   ```
   python sdsc_4107_project.py
   ```
2. The script will download data, train models, evaluate performance, and display plots for volatility prediction and interest rate forecasting.
## File Structure
- sdsc_4107_project.py: Main script containing all code for data processing, modeling, and visualization.
## Notes
- The script is self-contained and does not require additional configuration.
- For reproducibility, random seeds are set where applicable.
- The code is modular, with functions and classes for tail risk feature creation, modeling, and portfolio optimization.
## References
- S&P 500 data from Yahoo Finance
- Machine learning models: scikit-learn, TensorFlow, PyTorch
- Portfolio optimization: cvxopt
Feel free to further customize this README to match your project's specific goals or add more details as needed.
