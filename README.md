# Chandelier Exit from Pinescript to Python logic
PineScript to Python logic version of Chandelier Exit Indicator By Ji Hin

Original TradingView PineScript by Everget

## Chandelier Exit

The strategy was originally developed by Charles Le Beau and popularized by Dr. Alexander Elder in his book "Come Into My Trading Room: A Complete Guide to Trading" (2002) and converted into a indicator in TradingView by user Everget. It is a trailing Long and Short Stop indicator based on Average True Range (ATR). Some changes I made to the original script: 
* Built in conversion of normal Candlestick data into Heiken Aishi Candlestick data.
* Referenced https://www.youtube.com/watch?v=MNuZLHBYG9U and changed the ATR parameters to the ones stated in the video.
* Added a Zero Lag Least Squares Moving Averages (ZLSMA) as an extra indicator to double confirm the size of the position through the recommendation of the video.

## Data Visualisation
The final product is an exact copy of the Chandelier Exit indicator that also converts normal Candletick data into Heiken Aishi candlestick data, with ZLSMA indicator inclided, all visualised through Candlestick charts through plotly.graph_objects library. 

![Full Graph Picture](https://github.com/NJiHin/TA_Chandelier/blob/main/Graph%20pic.png)
*Full Graph picture*

![Zoomed Graph Picture](https://github.com/NJiHin/TA_Chandelier/blob/main/Zoomed%20in%20graph%20pic.png)
*Zoomed in Graph picture*


## Live Data

Implementation of live data from Unicorn Binance Websocket (https://pypi.org/project/unicorn-binance-websocket-api/) and fed into SQL Database. 

Script for Live Data is separated. 
