# Risk and Returns: The Sharpe Ratio
## Description
When you assess whether to invest in an asset, you want to look not only at how much money you could make but also at how much risk you are taking. The Sharpe Ratio, developed by Nobel Prize winner William Sharpe some 50 years ago, does precisely this: it compares the return of an investment to that of an alternative and relates the relative return to the risk of the investment, measured by the standard deviation of returns.

In this project, we will apply the Sharpe ratio to real financial data using pandas.
## Usage
Clone this repository and open the Jupyter notebook file (`*.ipynb`) in a Jupyter environment with Python kernel support. Make sure to install the required packages such as `pandas`, `numpy`, and `matplotlib`. You can do this by running the following commands in a code cell within the notebook:
```python
!pip install pandas numpy matplotlib
```
Once the packages are installed, run the code cells in the notebook to generate the plots and analyses.

If you don't have a Jupyter environment set up, you can install Jupyter Notebook and the Python kernel using the following steps:

1. Install Jupyter Notebook by following the instructions on the [official Jupyter website](https://jupyter.org/install).

2. Ensure you have Python installed. If not, you can download and install Python from the [official Python website](https://www.python.org/downloads/).
## Contents
1. **Meet Professor William Sharpe: Read in the stock data for Facebook, Amazon and the S&P 500.**
* Load stock and benchmark data from respective CSV files.
* Parse 'Date' column to datetime64, set it as index, and drop missing values.
2. **A first glance at the data: Take a peek at the data you loaded in the last task.**
* Display summary of each DataFrame using .info().
* Show first few lines of each DataFrame using .head().
3. **Plot & summarize daily prices for Amazon and Facebook: Plot and summarize the stock_data.**
* Display line plot of stock_data.
* Generate summary statistics for stock_data using .describe().
4. **Visualize & summarize daily values for the S&P 500: Plot and summarize the benchmark_data.**
* Display line plot of benchmark_data.
* Generate summary statistics for benchmark_data using .describe().
5. **The inputs for the Sharpe Ratio: Starting with Daily Stock Returns: Calculate, plot and summarize the stock_data returns.**
* Calculate daily returns using .pct_change().
* Display line plot of daily returns.
* Generate summary statistics for daily returns using .describe().
6. **Daily S&P 500 returns: Calculate, summarize, and plot daily returns for the benchmark_data.**
* Calculate daily returns for S&P 500 using .pct_change().
* Display line plot of S&P 500 daily returns.
* Generate summary statistics for S&P 500 daily returns using .describe().
7. **Calculating Excess Returns for Amazon and Facebook vs. S&P 500: Calculate, plot and describe the difference between stock_returns and sp_returns.**
* Calculate excess returns by subtracting sp_returns from stock_returns.
* Generate summary statistics for excess_returns using .describe().
8. **The Sharpe Ratio, Step 1: The Average Difference in Daily Returns Stocks vs S&P 500: Calculate and plot the mean of excess_returns.**
* Calculate the mean of excess_returns.
* Display a bar plot of the mean of excess_returns.
9. **The Sharpe Ratio, Step 2: Standard Deviation of the Return Difference: Calculate and visualize the standard deviation of excess_returns.**
* Calculate the standard deviation of excess_returns.
* Display a bar plot of the standard deviation of excess_returns.
10. **Putting it all together: Use avg_excess_return and sd_excess_return to calculate the Sharpe ratio, then annualize.**
* Calculate the daily Sharpe ratio.
* Calculate the annual factor using the square root of 252.
* Calculate the annualized Sharpe ratio.
* Display a bar plot of the annualized Sharpe ratio.
11. **Conclusion: Select the stock you would have picked in 2016 based on the Sharpe Ratio.**
*Set either buy_amazon or buy_facebook to True based on the calculated Sharpe Ratio.


