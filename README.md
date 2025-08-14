BTC

import yfinance as yf

btc = yf.download('BTC-USD', start='2014-09-17', end='2025-08-12')

btc.to_csv('bitcoin_complete_historical.csv')

ETH (synchronization)

eth_ticker_alt = yf.Ticker("ETHEREUM")

eth_data = eth_ticker_alt.history(period="max", interval="1d")

eth_complete_historical.csv

