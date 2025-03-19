# IBM Stock Price Prediction using LSTM

## Overview

This project implements an LSTM-based stock price prediction model to forecast hourly IBM stock prices (open, high, low, close) and trading volume for the next trading day. The model is trained on historical 5-minute interval stock data fetched from Alpha Vantage API and predicts stock behavior during trading hours (9 AM to 4 PM).

## Features

- **Real-time Data Fetching**: Retrieves IBM stock price data using the Alpha Vantage API.
- **Data Preprocessing**: Loads, cleans, and normalizes stock data using MinMaxScaler.
- **Sequence Creation**: Converts stock price data into sequences for LSTM model training.
- **LSTM Model**: A deep learning model designed to predict all key stock metrics for the next day's trading hours.
- **Visualization**: Graphs for predicted stock prices and volume trends.

## Installation & Dependencies

To run this project, ensure you have the following Python libraries installed:
- pandas
- scikit-learn
- numpy
- matplotlib
- tensorflow
- requests

## API Integration

The project uses the Alpha Vantage API to fetch real-time stock data. Replace `YOUR_API_KEY` with your actual API key.

## Usage

1. **Fetch Data**: Use the API to retrieve IBM stock data.
2. **Train the Model**: The script will preprocess data, train an LSTM model, and generate predictions.
3. **Get Predictions**: The model outputs hourly IBM stock prices and volume for the next trading day.
4. **Visualize Results**: The script generates plots to analyze stock trends.

## Visualization

- Predicted hourly stock prices (open, high, low, close) for the next day.
- Predicted stock trading volume.

## Contributing

Feel free to contribute by optimizing the model, improving visualization, or adding real-time data fetching capabilities.

## License

This project is open-source and available under the MIT License.

## Example Output

```plaintext
Predicted Next Day's Hourly Data:
      close    open    high     low   volume
9 AM  145.2   146.0   146.8   144.5  20000
10 AM 146.1   147.2   147.8   145.7  22000
...
