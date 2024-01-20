# Polygon-API-Automated-Data-Retrieval-and-Processing
Retrieved and processed price, dividend, and split data using the Polygon-API overwriting all erroneous data using a custom-made split adjustment file. Initial errors due to errors in polygon database.

#### Wrote sample functions to achieve the following goals:
1. Retrieve all ticker data from Polygon-API export into local csv files `get_tickers()`
2. Combine individual ticker data csv files into 1 ticker_data.csv `combine_tickers()`
3. Filter ticker_data.csv to include only relevant US exchanges as list `filter_us_exchange()`
4. Get bars (price data) for all relevant tickers from polygon-api as csv using `get_bars`
5. Get all split data from polygon-api as csv using `get_splits()`
6. Overwrite erroneous polygon_split.csv with manually made correct_splits.csv for relevant tickers using `fix_splits()`
7. Get all dividend data from polygon-api as csv using `get_divs()`
8. Combine all data into combine_bars.csv file for future adjustments  using `combine_bars()`
9. Fix all erroneous data using combined data frame and `adjust_bars()` function for proper price-split adjustments (essentially the main function)

### Check `Function Dictionary` category for detailed use of sample functions and their return values
