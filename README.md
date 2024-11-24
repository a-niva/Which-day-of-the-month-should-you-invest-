Performance Analysis of S&P500 Investment Strategies Based on Day of the Month
Overview

This project explores investment strategies based on the specific day of the month an investor chooses to make their investments in the S&P 500. The main goal is to analyze how investing on a fixed day of the month (e.g., the 1st, 2nd, etc.) impacts overall investment performance from 2010 to 2023.
Key Steps

    Data Collection:
        The dataset is retrieved using the yfinance library, fetching daily data for the S&P 500 index (^GSPC), including open, high, low, and close prices. The historical data spans from 2000 to 2023.

    Filtering the Data:
        The data is filtered for the period from January 1, 2000, to December 31, 2023, focusing on daily opening prices, which are used as the basis for analysis.

    Assigning the First Trading Day of Each Month:
        For each month, the first trading day (non-holiday weekday) is identified, which is used to align the data for each day in a given month. The goal is to find the corresponding first trading day for a specified day (e.g., the 1st, 2nd, etc.) across all months.

    Normalization:
        Each month's data is normalized relative to the first trading day, setting it to a base value of 100. This allows the performance to be compared across months, irrespective of the absolute price levels.

    Investment Strategy:
        An investment of $10,000 is made on the first trading day of each month. The strategy calculates the performance of these investments over time, tracking the number of shares bought and the total value of holdings.

    Performance Calculation:
        The performance (PERF) is calculated as the ratio of the total value of holdings to the total amount invested. The average performance for each chosen day (e.g., 1st day of each month, 2nd day, etc.) is also computed.

    Rankings and Visualization:
        The investments are ranked based on their performance (PALMARES). Various plots are generated to visualize the average performance over time and the rankings of each investment day across months.

    24-Month Moving Average:
        A 24-month moving average is applied to smooth the performance of each investment day, providing a clearer long-term trend.

    Heatmap and Stacked Bar Chart:
        The distribution of PALMARES ranks for each investment day is visualized using a heatmap. A stacked bar chart also shows the percentage distribution of ranks across the days of the month.

Data Sources

    S&P500 Data: The dataset is pulled from Yahoo Finance using the yfinance library. It includes daily open, high, low, and close prices of the S&P500 index (^GSPC).

Results

    Graphs: Several plots are generated to visualize the performance of investments for each chosen day of the month:
        Line Graphs: Show the average performance (AVG_PERF) for each day of the month.
        Rank Graph: Displays the ranking (PALMARES) of each day’s performance.
        24-Month Moving Average: Helps to analyze the smoothened performance trend for each day.
        Heatmap and Stacked Bar Chart: Provide insights into how frequently certain ranks appear for each investment day.

Requirements

To run this project, the following libraries are required:

    yfinance (for fetching financial data)
    pandas (for data manipulation)
    numpy (for numerical operations)
    matplotlib (for plotting graphs)
    seaborn (for advanced visualization)

pip install yfinance pandas numpy matplotlib seaborn

How to Use

    Install the necessary libraries as mentioned in the requirements section.
    Run the script in a Python environment (Jupyter Notebook, Python script, etc.).
    The script will fetch the S&P 500 data, process it, and output various performance graphs.

Example Visualizations

    Performance by Day: A line plot showing the average performance for each day of the month (e.g., Day 1, Day 2, ..., Day 31).
    Rankings: A plot visualizing the rankings of each day based on the average performance.
    24-Month Moving Average: A smoothened curve that helps identify long-term performance trends.
    Heatmap: A heatmap showing how each investment day fares in terms of ranks across months.

Conclusion

This project offers an in-depth look into how the timing of investments (on specific days of the month) impacts the long-term performance of the S&P 500 index. By analyzing historical data, it provides insights that can guide investors in selecting an optimal investment day each month.
