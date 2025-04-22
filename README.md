# Time Series Forecasting with RNN and LSTM

This project explores sequential modeling using **Recurrent Neural Networks (RNN)** and **Long Short-Term Memory (LSTM)** networks for time series forecasting tasks. It includes three main components:

## Simple RNN on Sine Wave Data

A Simple RNN model was built using 120 neurons and a Dense output layer to predict values from a synthetic sine wave dataset (0 to 6π). After preprocessing the data into sequences, the model was trained over 100 epochs with a batch size of 16.

**Result**: The model achieved a low MSE (~0.005), closely tracking the sine wave with minimal prediction error.

---

##  LSTM on Stock Price Data

An LSTM model was trained on IBM stock closing prices using 10-day lookback sequences. The architecture included two LSTM layers (50 units each), a dropout layer (20%), and a Dense output layer.

**Result**: After 100 epochs, the model showed strong generalization, with predicted prices closely matching actual values and validation loss stabilizing around 0.0028.

---

##  Redesigned LSTM for Improved Forecasting

To enhance prediction accuracy, the model was redesigned with:
- 3 LSTM layers (64 units each)
- Increased sequence length to 20 days
- Dropout rate increased to 30%
- Training epochs raised to 150

**Result**: Improved learning of long-term dependencies and reduced error by ~25%, demonstrating the impact of deeper architectures and longer historical context on forecasting accuracy.

---

## Summary

This project demonstrates:
- How Simple RNNs and LSTMs handle time-series data
- The impact of architectural design and hyperparameter tuning
- Visualization and evaluation of predictions through loss plots, residuals, and actual vs predicted comparisons
