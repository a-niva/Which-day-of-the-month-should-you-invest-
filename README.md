# S&P500 Investment Analysis

This project performs a detailed analysis of an investment strategy based on the S&P500 index data. The analysis focuses on the performance of investments made on specific days of each month (e.g., the 31st) over a period of time. The project utilizes historical data of the S&P500 index to evaluate performance, compute rankings, and visualize results.

## Overview

The primary goal is to explore the effects of investing on different days of the month (from 1st to 31st) and how these choices impact the overall performance over time. The project includes:

- Downloading S&P500 data from Yahoo Finance.
- Filtering and preparing the data.
- Normalizing the data for comparison across months.
- Performing investment simulations.
- Calculating the performance of investments based on various strategies.
- Plotting results to visualize trends and comparisons.

## Key Steps

### 1. Data Download and Preprocessing
- Download historical data for the S&P500 index using Yahoo Finance (`yfinance`).
- Filter data from the year 2000 to 2023.
- Normalize the data (e.g., adjust prices to a base of 100 for each month).

### 2. Investment Strategy Simulation
- Simulate investments made on specific days of each month (1st to 31st).
- Invest a fixed amount (e.g., 10,000 USD) on the chosen day.
- Track the performance of these investments over time, taking into account the price of the index on the day of investment.

### 3. Performance Calculation
- Calculate the total value of the investments.
- Calculate the performance as the change in value over the invested amount.
- Compute the cumulative performance over time and average performance for each day of investment.

### 4. Visualization
- Plot the average performance for each day of investment.
- Display rankings (`PALMARES`) of the performance for each month.
- Show the evolution of the rankings using line charts.
- Visualize the performance distribution using heatmaps and stacked bar charts.

### 5. Rolling Average
- Compute a 24-month rolling average for the performance rankings and visualize the trends for each day of investment.

### 6. Heatmaps and Stacked Bar Charts
- Visualize the number of occurrences of each position in the rankings for each day of investment.
- Display the results as a heatmap.
- Create an interactive stacked bar chart to represent the relative distribution of rankings.

## Libraries Used

- `yfinance`: To download S&P500 historical data.
- `pandas`: Data manipulation and analysis.
- `numpy`: Numerical operations.
- `matplotlib`: Plotting and data visualization.
- `seaborn`: Advanced plotting and heatmap generation.

## Key Functions

### `find_first_trading_day_for_month(year, month)`
Finds the first trading day of a given month and year.

### `assign_trading_day(year, month, day)`
Assigns the next available trading day if the given day is not a trading day.

### `normalized_data`
Contains the normalized S&P500 data (base 100) to compare prices across months.

### `investment_simulation()`
Simulates investments on a given day of each month, calculating the number of shares bought and the performance of the investment over time.

## Output

- **Performance Graph**: A line chart that shows the average performance (`AVG_PERF`) for each day of investment (1st to 31st).
- **Ranking Graph**: A graph showing the ranking (`PALMARES`) of each investment day across months.
- **Rolling Average Graph**: A graph showing the 24-month rolling average of performance rankings for each day of investment.
- **Heatmaps**: Visualizations of the counts of each ranking position for each day of investment.
- **Stacked Bar Charts**: Shows the relative percentage distribution of rankings for each day of investment.

## Example Graphs

### Performance of Investments

The first graph shows the average performance over time for each investment day.

![Performance Graph](performance_graph.png)

### Ranking of Days Based on Performance

The second graph displays the ranking of each day in the `PALMARES` across months.

![Ranking Graph](ranking_graph.png)

### 24-Month Rolling Average of Performance

The third graph shows the rolling average of the `PALMARES` over 24 months.

![Rolling Average](rolling_average_graph.png)

### Heatmap of Rankings

The heatmap visualizes the distribution of rankings for each day of investment.

![Heatmap](heatmap.png)

### Stacked Bar Chart of Positions

This stacked bar chart shows the percentage of positions within the `PALMARES` for each day of investment.

![Stacked Bar Chart](stacked_bar_chart.png)

## Requirements

- Python 3.x
- `yfinance`
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

To install the required libraries, use the following command:

```bash
pip install yfinance pandas numpy matplotlib seaborn



### Key Points to Customize:

- **Graph Image Links**: Replace the image placeholders (e.g., `performance_graph.png`) with the actual paths to your graphs if they are stored locally or on the web.
- **Additional Sections**: Add any other sections specific to your project (like data sources, additional features, or analysis results).
- **License**: If you’re using a specific license, adjust the License section accordingly.

This markdown provides a complete structure for documenting your project, including setup instructions, an overview of the analysis, and key visualizations.
