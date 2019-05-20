#########Code to create graph of SPY trends 
from quantopian.research import prices, symbols
import pandas as pd

##Graph of SPY closing prices from 2011 to 2015 
#Gets the closing price of SPY
spy_price = prices(symbols('SPY'),'2011-01-04','2015-01-04')
print(pd.DataFrame({
    'SP 500': spy_price
})).plot(title='S&P 500 Closing Price')

##Graph of SPY closing prices with 20 and 50 day moving average from 2011 to 2012
#Moving average of spy closing price
spy_price = prices(symbols('SPY'),'2011-01-04','2012-01-04')
spy_sma20 = spy_price.rolling(20).mean()
spy_sma50 = spy_price.rolling(50).mean()
#Print 
print(pd.DataFrame({   
    'SPY': spy_price,
    'SMA20': spy_sma100,
    'SMA50': spy_sma200
})).plot(title='S&P 500 Closing Price and Moving Average')
