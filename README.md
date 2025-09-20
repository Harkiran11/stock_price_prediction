# stock_price_prediction
Stock Price Prediction with PyTorch and LSTM

🚀 Features
Data retrieval from Yahoo Finance using yfinance

Data preprocessing and normalization

LSTM neural network implementation

Model training and evaluation

Visualization of predictions vs actual prices

Error analysis with RMSE metrics

## 🎯 What This Project Does
This project demonstrates how to build a neural network that predicts stock prices using historical data. It:

Downloads real stock data from Yahoo Finance

Uses an LSTM (Long Short-Term Memory) neural network

Predicts the next day's closing price based on previous days' data

Visualizes predictions compared to actual prices

Calculates prediction accuracy using RMSE (Root Mean Squared Error)

## 🔧 How It Works
### 1. Data Collection & Preparation
Uses yfinance library to download historical stock data

Focuses on daily closing prices

Normalizes data using StandardScaler for better training

### 2. Model Architecture
Built with PyTorch's LSTM layers

Input: Sequence of previous days' prices (default: 30 days)

Output: Prediction for the next day's price

Uses Mean Squared Error loss for training

Optimized with Adam optimizer

### 3. Training Process
Splits data into training (80%) and testing (20%) sets

Trains on historical sequences (look-back pattern)

Automatically uses GPU if available for faster training

Tracks and displays loss during training

## 4. Evaluation & Visualization
Calculates RMSE for both training and test data

Creates comparative plots showing actual vs predicted prices

Includes error analysis visualization

All results are converted back to original price scale for interpretation
