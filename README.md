# Apple Stock Price Prediction using LSTM

This project implements a Long Short-Term Memory (LSTM) neural network to predict Apple stock prices based on historical data. The model is trained on Apple stock data from 2012 to 2019 and uses 60-day price windows to make predictions.

## Overview

This project:
- Fetches historical Apple stock data using pandas-datareader
- Preprocesses and scales the data for LSTM modeling
- Builds and trains a sequential LSTM model
- Evaluates model performance on test data
- Visualizes predictions against actual stock prices
- Predicts future stock prices based on recent trends

## Technologies Used

- Python 3
- TensorFlow & Keras
- Pandas & NumPy
- Scikit-learn
- Matplotlib
- pandas-datareader

## Model Architecture

The LSTM model architecture consists of:
- First LSTM layer with 50 neurons, returning sequences
- Second LSTM layer with 50 neurons, not returning sequences
- Two Dense layers with 25 and 1 neurons respectively
- Adam optimizer with mean squared error loss function

## Results

The model provides predictions for Apple's stock prices and calculates the Root Mean Squared Error (RMSE) to evaluate prediction accuracy. Results are visualized to compare actual vs predicted stock prices.


## Future Improvements

- Increase the training epochs for potentially better accuracy
- Experiment with different window sizes (currently using 60 days)
- Implement additional features beyond just closing price
- Try different model architectures and hyperparameters
- Add backtesting framework to evaluate trading strategies

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Yahoo Finance for providing the historical stock data
- TensorFlow and Keras documentation for LSTM implementation guidelines
