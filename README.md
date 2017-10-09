# WordMath

Assignment 4: Pandas & Stock Analysis IS590PR

Review Chapter 4 of McKinney’s book and the Jupyter Notebook we looked at in class by Shubhanshu Mishra here: https://github.com/napsternxg/DataAnalysisPython

Borrowing ideas from those sources, create a well-documented Python script (not a Jupyter Notebook) with modular design (broken up into sensible functions) and some Doctests, that does the following:

1. Define a dictionary of names and “tickers” for some major stock indexes. Include these: a. NASDAQ Composite: “COMP” b. NYSE Composite: “NYA” c. Dow Jones Industrial Average: “DJIA” d. S&P 500: “SPX” e. S&P Asia 50 ETF: “AIA” f. Euro STOXX 50: “FEZ”

2. Ask the user to type in a list of any individual stock tickers. For example, they might enter “IBM, MSFT, ORCL, CSCO, XOM”.

3. Automatically download the stock data for the past 24 months (up to current date), from Yahoo (as shown in the examples) for all listed tickers.

4. Your program should load all those stock price histories into a Pandas DataFrame. Specifically, we’ll use the “adjusted close” prices.

5. Then, calculate the correlations between each of the input tickers against each Index. 

6. Output a result that shows which index correlates most strongly with each individual stock and vice versa.

7. Make use of the Pandas shift() method to help calculate whether any of the stocks correlate more strongly with an index when shifted anywhere in the range up to 5 days earlier or later. Output the strongest finding for each combination, only if they exceed the date-aligned ones calculated previously. Although such a finding does not prove any predictive causation between the prices, it’s an interesting conjecture to explore further, if any high correlation is discovered.

Optional bonus credit: Using either the matplotlib or seaborn library, generate a line graph of the data above (ignoring step 7). It should have a separate line for each ticker’s price, with x-axis the date and y-axis the price.
