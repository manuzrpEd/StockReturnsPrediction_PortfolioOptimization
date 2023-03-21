# Investment Porfolio Optimization



This repo is inspired and adapted from: <a href="https://github.com/georgemuriithi/investment-portfolio-optim">
https://github.com/georgemuriithi/investment-portfolio-optim
</a>.


I create an investment portfolio of stocks using LSTM and XGBoost stock returns predictions and optimizing portfolio weights. The performance of this portfolio is better compared to an equally weighted portfolio.

![Performance](https://user-images.githubusercontent.com/69723856/226715865-3aa25c2c-bb8f-433e-90a8-a9850aa46dc1.png)

***Disclaimer:** The LSTM or XGBoost models cannot be used to predict stock returns in real life and this project cannot help you make investment decisions in the stock market. The stock market is highly unpredictable, therefore, prediction models do not work. In this project, the validation phase is used for analysis. The purpose of this project is to implement **Univariate Time-Series Prediction using LSTM & XGBoost.***

## Problem Description
An investment portfolio of several stocks is made by making their price predictions using an **LSTM Univariate Time-Series Prediction** model. Then, daily returns are computed from the predicted stock prices and used to get the weights that maximize overall return. This is done through **SLSQP (Sequential Least SQuares Programming)** optimization.

### Data
The **top 30 U.S. companies by market capitalization** are used. The start time is **2009-12-31** and the end time is **2021-12-31.** AbbVie (ABBV), Meta (FB) and Tesla, Inc. (TSLA) are excluded because they were listed in the stock market after 2009-12-31.

The csv files and model states can be accessed from the *data* folder.
