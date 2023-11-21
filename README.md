# Genesis EA - ReadMe

This ReadMe file provides an overview and explanation of the Genesis EA code. Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that can work as described in the product. To find the official developer of this product, please refer to MQL5.

## Table of Contents
- [About](#about)
- [Custom Functions](#custom-functions)
- [Initialization](#initialization)
- [Tick Function](#tick-function)
- [Deinitialization](#deinitialization)

## About
The Genesis EA is a trading robot developed by the Forex Robot Easy Team. The EA is designed to trade on the Forex market and aims to identify potential reversals in the trend.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/review-genesis-ea-a-professional-forex-traders-perspective-on-the-modern-trading-system/).

## Custom Functions
The Genesis EA includes several custom functions that are used throughout the code. These functions are:

- `OpenOrder(int direction)`: This function is used to open a new order with the specified direction (1 for buy, -1 for sell).
- `CloseSeries()`: This function is used to close all orders in the current series.

## Initialization
The initialization function `OnInit()` is called when the EA is initialized. It performs the following tasks:

- Checks if the symbol is valid (EURUSD, AUDUSD, AUDCAD, EURGBP, GBPUSD, GBPCAD, GBPCHF).
- Checks if the timeframe is valid (H1).
- Sets the magic number for the orders.

## Tick Function
The tick function `OnTick()` is called on every tick of the market. It performs the following tasks:

- Gets the current price and the previous price.
- Checks if the trend is ready to reverse based on the average overbought/oversold value.
- Opens a new order if the conditions are met, considering the maximum number of orders in the series.
- Checks if the series of orders needs to be closed based on the profitability of the orders.

## Deinitialization
The deinitialization function `OnDeinit(const int reason)` is called when the EA is deinitialized. It performs the following tasks:

- Closes any remaining open orders in the series.

For more details on the functionality and trading results of the Genesis EA, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/review-genesis-ea-a-professional-forex-traders-perspective-on-the-modern-trading-system/).
