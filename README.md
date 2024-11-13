# Portfolio Optimization and Forecasting

This project demonstrates a data-driven approach to optimize an investment portfolio using historical data for three assets: **Tesla (TSLA)**, **Vanguard Total Bond Market ETF (BND)**, and the **S&P 500 ETF (SPY)**. Using advanced time series forecasting and optimization techniques, we aim to maximize returns while controlling for risk.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Collection and Preparation](#data-collection-and-preparation)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [Time Series Forecasting](#time-series-forecasting)
5. [Portfolio Optimization](#portfolio-optimization)
6. [Results](#results)
7. [Future Work](#future-work)
8. [Technologies Used](#technologies-used)
9. [Getting Started](#getting-started)

## Introduction
In a dynamic financial landscape, effective portfolio management is key to achieving long-term investment goals. This project leverages historical data and time series forecasting to optimize a portfolio that balances risk and return.

## Data Collection and Preparation
- **Assets Analyzed**: Tesla (TSLA), Vanguard Total Bond Market ETF (BND), S&P 500 ETF (SPY)
- **Data Source**: Yahoo Finance
- **Time Period**: January 1, 2015 – October 31, 2024

Data preprocessing steps included handling missing values, scaling data, and preparing it for time series modeling.

## Exploratory Data Analysis (EDA)
Key insights from EDA:
- **Trend Analysis**: Notable upward trends in TSLA, BND, and SPY with varying volatility levels.
- **Volatility Analysis**: TSLA showed the highest volatility; BND, the least.
- **Seasonality and Trend Decomposition**: Patterns revealed for more effective forecasting.

## Time Series Forecasting
Three models were evaluated to forecast asset prices:
- **ARIMA**: Effective for stationary data.
- **SARIMA**: ARIMA with seasonality.
- **LSTM**: Captures long-term dependencies in data.

### Model Training and Evaluation
- Data split into training and testing sets.
- **Parameter Optimization**: ARIMA and SARIMA parameters tuned using grid search; LSTM optimized for epochs and sequence length.
- **Best Model**: LSTM performed best in forecasting future trends.

## Portfolio Optimization
Initial portfolio weights were evenly distributed among the three assets. To enhance returns while controlling risk, the portfolio was optimized for the **Sharpe Ratio** under constraints.

### Optimized Weights
- **TSLA**: 9.96%
- **BND**: 65.45%
- **SPY**: 24.60%

## Results
The optimized portfolio has:
- **Expected Annual Return**: 20.40%
- **Portfolio Volatility**: 21.95%
- **Sharpe Ratio**: 0.88

This composition increases allocation to BND, enhancing portfolio stability while balancing risk and growth.

## Future Work
- Experiment with additional forecasting techniques, such as Prophet and machine learning models.
- Explore sentiment analysis to integrate market sentiment into forecasts.
- Incorporate transaction costs and taxes to refine real-world applicability.

## Technologies Used
- **Python**
- **Libraries**: pandas, NumPy, scikit-learn, statsmodels, TensorFlow/Keras (for LSTM)
- **Data Source**: Yahoo Finance API

## Getting Started
To replicate this project:
1. Clone the repository.
2. Install required dependencies: `pip install -r requirements.txt`
3. Run the data collection and preprocessing scripts.
4. Experiment with forecasting models and portfolio optimization scripts.

For detailed steps and code examples, refer to the project files.

---

Feedback and contributions are welcome!
