- Author:(20/01) MScFE 690 Capstone (C18-S3T5)   Ernest Osifo
- Email: osifo.e@gmail.com
- Date: 4 April 2020 
PROJECT: CRYPTOCURRENCY TRADING-PAIR FORECASTING, USING MACHINE LEARNING AND DEEP LEARNING TECHNIQUE
Version of Python: 3.6.5
## Description
In this project, we attempt to forecast cryptocurrency price and design a strategy that will take advantage of the statistical arbitrage via paired crypto-currency trading.
Our task is divided into the following three major steps (Two Phases)

Phase 1.: Get the Pair currencies; Find the most correlated cryptocurrency to our base Currency (Bitcoin) 
Phase 2.: Forecast Adjusted price for selected pair & Develop a proposed trading strategy 

Phase 1: 

Six Hundred and Ten days was used for the search for a pair for Our paired Trading.
The period and stock considered are:
610 days of Adjusted Close, Cryptocurrencies , 1 Jan 2018 to 1 Sept 2019.
(Sourced data from: Yahoo finance.)
## Data Analysis Jupyter Notebook
The following data analysis is performed on our Choice base currency, Bitcoin (BTC) and Eight others 
Source: The top ten Cryptocurrencies as at 8 October 2019 noted by Yahoo Finance (https://finance.yahoo.com/news/top-10-cryptocurrencies-market-capitalisation-160046487.html)

1. Bitcoin (BTC)
2. Ethereum (ETH)
3. XRP (XRP)
4. Bitcoin Cash (BCH)
5. Tether (USDT)
6. Litecoin (LTC)
7. EOS (EOS)
8. Binance Coin (BNB)
9. Bitcoin SV (BSV); the BSV has no unique ticker in yahoo finance (and claims to be the original version of what Bitcoin was meant to be; Source: https://bitcoinsv.com/en/learn)
10. Stellar (XLM)

Methodology 
1. from Yahoo finance, downloaded the Adjusted Close price
2. Concatenated the Adjusted Close price, calculated the Percentage returns and the cumulative returns
3. Compute correlation and Cointegration of returns for the cryptocurrencies. 
4. the Spread for the pairs were also examined.
5. Selection of the best fit pair was done based on the Compute correlation and Cointegration of returns.

The pair selected will be used for phase 2 of the project; (Price forecasting and developing a mean-reverting, pair-trading strategy)

JUPYTER NOTEBOOK:
1. CRYPTOCURRENCY TRADING-PAIR FORECASTING, USING MACHINE LEARNING AND DEEP LEARNING TECHNIQUE (PART1&2)


Notes:
run the Jupyter notebook from the desktop of your computer with an active internet connection.
to run from any other location, you might need to kindly adjust this family of codes

BTC.to_csv(r'.\BTC.csv',index='Date') 
ETH.to_csv(r'.\ETH.csv',index='Date')
in order for you to generate the csv files.
while running this jupyter notebook, it will generate and save 2 csv files on the directory path 
. Bitcoin (BTC)  
. Ethereum (ETH), 

The Speed of processing data is heavily dependent on the computational speed and network connectivity, running the complete package might take a while.


## Packages Used
 	numpy==1.14.2
 	pandas==0.22.0
 	Cython==0.28.2
 	glob,os
 	matplotlib.
 	Statsmodels
 	coint_johansen
 	keras.models 
 	pmdarima.arima 
 	sklearn.preprocessing 
 	MinMaxScaler
 	Scipy
 	arch.unitroot 
## Notes: 
* This program was built using a Dell Latitude E6430 on Windows Operating System.
* Python 3.6.5 was used
* Tested Successfully on Windos OS
* The codes might take some time to proccess ( about 15 Minutes)  depending on the computational speed of your computer 

* Project complete work is accessable in a attached PDF named: (20 JAN) MScFE 690 Capstone (C18 S3T5) Group 10)



Copyright (c) 2020 Osifo Ernest 

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and  associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

