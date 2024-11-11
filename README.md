# Stock Market Time Series Analysis

This repository contains a Python notebook for performing time series analysis on historical stock market data. The analysis is focused on Google's stock (GOOG) and includes data collection, preprocessing, visualization, and the application of ARIMA (AutoRegressive Integrated Moving Average) and SARIMAX models for making predictions.

## Project Workflow

<img src = "/workflow.jpeg">

### Importing Libraries

In this section, necessary Python libraries such as pandas, yfinance, and datetime are imported for data handling and time series analysis.

### Data Collection

This section retrieves historical stock market data for Google (GOOG) from Yahoo Finance API. It defines the date range for data collection and selects relevant columns.

### Data Preprocessing

Here, the data is further preprocessed. It narrows down the dataset to include only the 'Date' and 'Close' columns. The code also resets the index for data consistency.

### Data Visualization

This section uses the matplotlib library to create a time series plot of the closing prices of Google's stock. The 'fivethirtyeight' style is applied for visualization.

### Time Series Decomposition

The statsmodels library is utilized for seasonal decomposition. This cell separates the trend, seasonality, and residual components of the stock prices.

### AutoCorrelation Plot

AutoCorrelation is visualized using the pandas library, helping identify potential time series patterns.

### Partial AutoCorrelation Plot

This cell generates the Partial AutoCorrelation Function (PACF) plot to aid in parameter selection for the ARIMA model.

### ARIMA Modeling

The ARIMA (AutoRegressive Integrated Moving Average) model is constructed here. It fits the model to the 'Close' prices with specified parameters and prints a summary of the model.

### ARIMA Predictions

This cell generates predictions using the ARIMA model and prints the results.

### SARIMAX Predictions

Predictions for future stock prices are generated using the SARIMAX model.

### Data and Predictions Visualization

The cell plots the training data and the predictions on a single graph for visual comparison.

## Getting Started

To run the notebook and perform your own analysis, you can follow these steps:

1. Ensure you have Python installed on your system.

2. Install the required libraries by running:

   ```
   pip install -r requirements.txt
   ```

3. Clone this repository to your local machine:

   ```
   git clone https://github.com/subhan-liaqat/Google-Stock-Price-Prediction-using-ARIMA-Model
   ```

4. Open the Jupyter notebook in your favorite Python environment (e.g., Jupyter Notebook, Jupyter Lab) and run each cell to analyze the stock market data.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The analysis was performed using Python and popular data science libraries.
- Historical stock market data was obtained from Yahoo Finance.
