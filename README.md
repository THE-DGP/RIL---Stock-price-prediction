# Project Overview
This python program uses various libraries to process historical stock prices of Reliance Industries Ltd. 
It simply predicts whether the stock price will go up or down.
# Steps
### 1. Downloading Reliance Industries ltd. data
     1. Import yfinance, i.e. Yahoofinance API
     2. search for the symbol of company, for reliance it is RELIANCE.NS
     3. create DataFrame

### 2. Data cleaning
    1. Remove coloumns that are not required (dividends, stock splits)
    2. Plot the graph of closing prices against index

### 3. Setting target for learning 
    Target is a coloumn that has 1 for everytime stock price was higher than the previous day and 0 otherwise.

### 4. Training Model
    1. Using RandomForestClassifier for machine learning
    2. Take into consideration very recent historic stock price data to get better results
    3. Very Old trends have almost zero significance in prediction

### 5. Backtesting
    We will create a function where we will first predict for (n+1)th year on basis of 'n' years

### 6. Using additional predictors
    1. Here we take ratios of closing prices of 2 and 5 days, 5 and 60 days, and so on. (trend ratio analysis)
    2. Now we will have lesser number of days when the algorithm predicts rise in stock price

# Requirements
1. Jupyter Notebook
2. Python 3.8+
3. Python packages
    1. Pandas
    2. yfinance
    3. scikit-learn

# Dataset 
The Data used will be directly accessed through <a href="https://pypi.org/project/yfinance/" target="_blank">yfinance</a>
