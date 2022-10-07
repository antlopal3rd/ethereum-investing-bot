# ethereum-investing-bot
An algo trading bot to buy and sell ethereum in the 4h timeframe. It uses the Binance API to obtain both historic and live price data.

### Requirements:

 websocket-client, rel, python-binance, TA-Lib, pandas, numpy, matplotlib
 
 ### Setup:
 
 After installing all required packages you will need to go to your Binance account and obtain your API keys. You can save them in a txt file and read them from the code.
 
### Live chart:

In the first file called *realtimedata_plot.ipynb* you can find the code for an interactive matplotlib chart that updates every second with the price data fed by the API. You can change this line of code to display another different asset:
```
symbol = "ETHUSDT"
```
At the end of the file you can find commented code for those wanting to save s hort video of the live chart.

### Live connection with historic prices:

In the second file called *liveconnection_numpy.ipynb* you can find the code that creates several numpy arrays with both historic and live data in order to build the trading bot that manages real money. You can change the timeperiod and asset name to your liking.

### Main strategy and charting:

In the third file called *main_strategy.ipynb* you can find the rules for 
