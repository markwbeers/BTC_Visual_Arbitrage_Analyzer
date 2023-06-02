
# Module 3 Challenge - Crypto Arbitrage

apply the three phases of financial analysis to determine if any arbitrage opportunities exist for Bitcoin on the BTSP and COIN exchanges.

## Technologies

The code is written to run in the 'dev' environment we set up in Python version 3.7.1, (now running python version 3.10.9.final.0) on a [JupyterLab](https://jupyter.org) Notebook (version 3.4.4).

## Libraries and Packages:

+ *'[pandas](https://pandas.pydata.org/)'* (used for data manipulation and analysis)
+ pathlib: *'Path'* which is a class included as part of the 'pathlib' module in Python's standard library is needed to import data with the "read_csv" command.
+ %matplotlib.pyplot - inline (used for data visualizations; displays plots inline with code instead of writing to another file or other output option)

## Collect the data:

pd.read_csv() - Used to read data from a CSV file and create a DataFrame.

## Prepare the data:

dropna() - Used to drop rows or columns containing missing values from a DataFrame.
str.replace() - Used to replace a substring or pattern in a string column with another value.
astype() - Used to change the data type of a column in a DataFrame or Series.
isnull() - Used to check for missing values in a DataFrame or Series and returns a boolean mask indicating which values are missing.
duplicated() - Used to identify duplicated rows in a DataFrame and returns a boolean mask indicating which rows are duplicates.
head() - Used to return the first n rows of a DataFrame.
tail() - Used to return the last n rows of a DataFrame.

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


---

## Usage

1) navigate to my github repo called "3_crypto_arbitrage_BTC_BTSP_COIN" and activate your 'dev' environment for python 3.7
2) clone the repo locally and open a jupyter lab notebook in the folder "3_crypto_arbitrage_BTC_BTSP_COIN"
3) the code is in `crypto_arbitrage.ipynb` 

Finally, run the code from *Jupyter Notebook* in your browser.

---

## Contributors

Mark Beers: 
[Linked In](https://www.linkedin.com/in/markwbeers/)
---

## License

MIT License: A short and simple permissive license with conditions only requiring preservation of copyright and license notices. Licensed works, modifications, and larger works may be distributed under different terms and without source code.