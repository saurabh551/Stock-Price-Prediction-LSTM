# Stock Price Prediction using LSTM

A time-series forecasting project that uses a stacked Long Short-Term Memory (LSTM) neural network to model historical Apple (AAPL) closing prices and generate a 30-step future forecast.

## Features

- Historical AAPL closing-price visualization
- Train/test split for time-series data
- Min-Max normalization fitted on training data
- 100-timestep sequence generation
- 3-layer stacked LSTM model
- Training and validation loss visualization
- RMSE evaluation on training and test data
- Recursive 30-step forecasting

## Tech Stack

Python, TensorFlow, Pandas, NumPy, Matplotlib, Scikit-learn, LSTM

## Repository Structure

```text
Stock-Price-Prediction-LSTM/
├── README.md
├── stock_price_prediction_lstm.ipynb
├── requirements.txt
├── .gitignore
└── data/
    └── AAPL.csv
```

## Dataset

The notebook expects:

```text
data/AAPL.csv
```

with a `close` column. The original project data also contains fields such as `date`, `open`, `high`, `low`, and `volume`.

Place the dataset in `data/AAPL.csv` before running locally.

## Run in Google Colab

[Open the notebook in Google Colab](https://colab.research.google.com/github/saurabh551/Stock-Price-Prediction-LSTM/blob/main/stock_price_prediction_lstm.ipynb)

The notebook also contains a GitHub Raw URL fallback for `data/AAPL.csv`.

## Evaluation

Because this is a regression problem, the notebook evaluates the model using Root Mean Squared Error (RMSE).
