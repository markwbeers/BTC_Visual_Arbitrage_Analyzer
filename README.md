# Module 3 Challenge - Crypto Arbitrage

##Apply the three phases of financial analysis to determine if any arbitrage opportunities exist for Bitcoin on the BTSP and COIN exchanges.

## Bitcoin Arbitrage and 'day trading' the firms holdings - **report to VP of Currency Trading at UCB FinTech Investors Fund**

+ Bitcoin is a volatile currency and long term holdings without active hedging strategy is far too risky for our firm's assets.
+ [Bitcoin Fell 50% in the 1st Quarter of 2018](https://totalbitcoin.org/q1-2018-btc-fell-50-percent/)
+ Based on researching arbitrage opportunities in several exchanges, we chose [**Bitstamp**](https://www.bitstamp.net/) and [**Coinbase**](https://www.coinbase.com/) as dependable and competent exchanges.
+ Trading costs of 1% are reasonable and exchange imbalances arise in particular volatile trading runs and open opportunities to profit.
+ Our analysis of 3 specific dates and one 3 day window indicate large potential for scalping different exchange imbalances.
+ Timing trades is key to success and we are researching what events and other national news, Fed reports, world events, etc. may have coincided with the arbitrage opportunities found in Q1 of 2018.  
+ We recommend the firm continues this research and to analyze more external data on a timeline as well as potential [**other exchanges for BTC**](https://bitcoin.org/en/exchanges)

Collect CSV data in a Jupyter notebook file.
Prepare the datasets for analysis by cleaning missing and erroneous data.
Analyze the data at a high level through summary statistics and visualizations, and use this information to select areas for deeper analysis. Specifically, you’ll select time periods in which to identify arbitrage opportunities.

## Technologies

The code is written to run in the 'dev' environment we set up in Python version 3.7.1, (now running python version 3.10.9.final.0) on a [JupyterLab](https://jupyter.org) Notebook (version 3.4.4).

In order to ensure plot visualals remain intact for any viewer, the code references hexcodes from ['216 web-safe colors Chart from ColorHexa'](https://www.colorhexa.com/web-safe-colors)

## Libraries and Packages:

+ *'[pandas](https://pandas.pydata.org/)'* (used for data manipulation and analysis)
+ [pathlib](https://docs.python.org/3/library/pathlib.html): *'Path'* which is a class included as part of the 'pathlib' module in Python's standard library is needed to import data with the "read_csv" command.
+ [%matplotlib inline](https://pypi.org/project/matplotlib-inline/) (uses for data visualizations; displays plots inline with code instead of writing to another file or other output option)

## Collect the data:

pd.read_csv() - Used to read data from a CSV file and create a DataFrame.

## Prepare the data:

        **dropna()** - Used to drop rows or columns containing missing values from a DataFrame.
        **str.replace()** - Used to replace a substring or pattern in a string column with another value.
        **astype()** - Used to change the data type of a column in a DataFrame or Series.
        **isnull()** - Used to check for missing values in a DataFrame or Series and returns a boolean mask indicating which values are missing.
        **duplicated()** - Used to identify duplicated rows in a DataFrame and returns a boolean mask indicating which rows are duplicates.
        **head()** - Used to return the first n rows of a DataFrame.
        **tail()** - Used to return the last n rows of a DataFrame.

## Analyze the data:

plot() - Used to create various types of plots, such as box plots and line plots.
sum() - Used to calculate the sum of elements in a DataFrame or Series.
cumsum() - Used to calculate the cumulative sum of elements in a DataFrame or Series.

---

### Classes/Object Types:

    + Series (one dimensional labeled object consisting of 'data values' and an 'index' used to store and manipulate data
    + DataFrame (a two-dimensional labeled data structure in pandas, used to store and manipulate data)
    + Path (used with read_csv function represents a file or directory path)

### Methods/Attributes/Functions:

    + dtypes attribute (to view the data types of columns in a DataFrame)
    + read_csv() function (used to read a CSV file into a DataFrame)
    + head() used to view the first few rows of a DataFrame
    + tail() used to view the last few rows of a DataFrame
    + plot() method creates various types of plots, such as box plots and line plots
    + sum() method to calculate the sum of elements in a DataFrame
    + cumsum() method to calculate the cumulative sum of elements in a DataFrame
    + isnull() method to check for null values in a DataFrame
    + sum() method to calculate the sum of elements in a DataFrame
    + dropna() method to drop rows with empty, NaN, or null values from a DataFrame
    + str.replace() method to replace characters and/or substrings in a string
    + astype() method to convert the data type of a column in a DataFrame
    + duplicated() method to check for duplicate rows in a DataFrame
    + copy () method allows creation of a separate copy of an object to manipulate as needed for use while preserving the origina
    
### Variables Used:

standard Python variables, such as integers, floats, and strings. Code mainly focuses on utilizing the pandas library's DataFrame object to manipulate and analyze data, and the matplotlib library's pyplot module to create visualizations.

---

## Installation Guide

Pandas and matplotlib are likely installed with a full [Anaconda Installation](https://docs.anaconda.com/free/anaconda/install/windows/), however, if you're not sure just activate your `dev` environment as python 3.7 and check:

```
            
            **$ conda list pandas**

               Name                    Version                   Build  Channel
            pandas                    1.3.5            py37h6214cd6_0

            **$ conda list matplotlib**

               Name                    Version                   Build  Channel
            matplotlib                3.5.2            py37haa95532_0
            matplotlib-base           3.5.2            py37hd77b12b_0
            matplotlib-inline         0.1.6            py37haa95532_0

```
if do not have, use pip install.

            pip install pandas
            pip install matplotlib

---
## Usage

1) navigate to my github repo called "3_crypto_arbitrage_BTC_BTSP_COIN" and activate your 'dev' environment for python 3.7
2) clone the repo locally and enter 'git pull' to import the files locally.
3) open a jupyter lab notebook in the folder "3_crypto_arbitrage_BTC_BTSP_COIN" - code is in `crypto_arbitrage.ipynb` 
4) type **`jupyter lab 3_crypto_arbitrage_BTC_BTSP_COIN`** at the prompt in your terminal or gitbash prompt $ 
5) you may open the .csv files to check out in the "Resources" subfolder

Finally, run the code from *Jupyter Notebook* in your browser.

### Coding Style - DRY and versatile - Hope the VP can code in python!! 

+ to change dates for analysis, select the end tag of a dataframe carrying the date, highlight the **'MMDD'** with the cursor.
+ hold `Ctrl-F` and then choose `Replace` to swap in a different date from Q1 2018 to experiment with the data, it should fully update all relevant data frames and effectively allow for fast recoded manipulation of data.
+ variables have also been shortened so the many manipulated DataFrames can be tracked and rewritten quickly to modify code.
+ With the 3 day date window **EXTRA** section at the end of the notebook, a different range can quckly be sliced up for multiple date runs.
    
## Additional Notes/Suggestions to VP for manipulating code and use of formulas to calculate desired arbitrage points and BTC source for purchase.
       + most trade dates are not clear winners/losers to purchase only from one exchange and sell to the other exclusively.  
       + many dates will likely show a 'mean' close to zero and one sided buying or selling on a given day is not a good daily strategy.
       + data frames needed to manipulate and flip exchanges to rework visualizations are easily flipped.
       + try using Find/Replace on "COIN" and "BTSP" to toggle where seems appropiate use method `Ctrl-F` and then choose `Replace`
       + review specific notes below prior to any code manipulation
       
### "rule of thumb" ways to understand and manipulate formulas

**swap out "_coin" for "_btsp" or vice versa when manipulating data** 
since the x-axis on the visualization is also the "Timestamp" index - look for patterns to see if advantages to trading only near opening and/or closing.

**'creating arbitrage DataFrames'**
subtract the lower-priced exchange from the higher-priced one to find our *arbitrage spread* for any given date or range of dates.

**'calculate spread returns' - Step #4 / Part 2**
      "divide the instances that have a positive arbitrage spread (that is, a spread greater than zero) ... from the exchange you’re buying on ... the lower-priced exchange)"
**'calculate potential profit'- Step #4 / Part 5**
      "multiply the spread returns that were greater than 1% by the cost of what was purchased"

---

## Contributors

Mark Beers: 
[Linked In](https://www.linkedin.com/in/markwbeers/)
---

## License

MIT License: A short and simple permissive license with conditions only requiring preservation of copyright and license notices. Licensed works, modifications, and larger works may be distributed under different terms and without source code.