# Monthly Investment Returns Analysis

This project analyzes the returns of a monthly investment made on different days of the month using historical stock market data (e.g., the S&P 500 index). It helps evaluate which day of the month provides the best returns for regular investments, and visualizes the results using various plots.

## Objective

The goal of this project is to determine which day of the month (from 1 to 31) generates the best total returns for a regular monthly investment, based on historical market data. The project provides visualizations of cumulative returns in bubble chart form to better understand performance.

## Features

- **Investment Return Calculation**: Analyzes the growth of invested capital on different days of the month.
- **Visualization**: Bubble charts depicting total returns for each investment day.
- **Parallelization**: Uses `joblib` to parallelize calculations and speed up data processing.

## Installation

### Prerequisites

Make sure you have Python 3.x installed on your system along with the following libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `joblib`
- `yfinance` (for fetching historical data)

You can install the necessary packages using `pip`:



Usage

The main goal of this analysis is to examine how the returns vary depending on the day of investment within each month. The results will be plotted in a bubble chart that shows:

    X-axis: Days of the month (1-31)
    Y-axis: Cumulative returns (%)
    Bubble size: Total return for that investment day

This helps to identify patterns and trends in the market that might suggest the best days for regular investments.

This project is licensed under the MIT License - see the LICENSE file for details.
