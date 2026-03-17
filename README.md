# Mathematical Analysis of Stock Market Volatility and Portfolio Vectors

## 🎯 Project Objective
This project applies **Linear Algebra**, **Multivariate Calculus**, and **Statistical Analysis** to financial time-series data. The goal is to mathematically model the relationship between risk and return to determine an "optimal" asset allocation.

## 📈 Problem Formulation
We treat a collection of stocks as a **multidimensional vector space** where:
*   **Calculus**: We calculate the "velocity" of price movements via daily percentage changes (the first derivative of price).
*   **Statistics**: We analyze the correlation and covariance between these vectors to identify diversification benefits.
*   **Optimization**: We seek a weight vector $W$ that minimizes a custom cost function (variance) while satisfying real-world constraints.

## 🧠 The "Math Strategy": Risk Aversion Coefficients
Unlike standard models that only look at mean-variance, this system incorporates **Higher-Order Moments** (Skewness and Kurtosis) to account for "Black Swan" events and tail risk.

The optimizer's behavior is governed by these **Risk Aversion Coefficients**:
*   **`lambda_var` (0.5)**: Penalty for Volatility (Standard Deviation).
*   **`lambda_skew` (0.1)**: Reward for Positive Skewness (favoring "right-leaning" returns).
*   **`lambda_kurt` (0.2)**: Penalty for Kurtosis (protecting against extreme tail risk).

## 🛠 Methodology
The project follows a rigorous scientific workflow:
1.  **Data Acquisition**: Extracting historical market data via APIs.
2.  **Mathematical Modeling**: Defining the vector space and risk parameters.
3.  **Implementation**: Coding optimization algorithms in Python.
4.  **Validation**: Backtesting against historical "unseen" data.

## 🚀 Technologies Used
*   **yfinance**: Financial data extraction.
*   **Pandas & NumPy**: Matrix operations and data manipulation.
*   **Matplotlib & Seaborn**: Statistical visualization.
*   **SciPy (stats)**: Calculation of Skewness and Kurtosis.

## 💻 Installation & Dependencies

  To run this project, you will need to install the following Python libraries:

  pip install yfinance pandas numpy matplotlib seaborn scipy

---
