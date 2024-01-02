# Trading Simulator in StrategyTester

This is a trading simulator code designed to be run in the MetaTrader 5 Strategy Tester. It allows users to test and optimize their forex trading strategies before implementing them in live market conditions. 

## Inputs

The code requires the following inputs:

- StopLoss: The desired stop loss in points.
- TakeProfit: The desired take profit in points.
- OrderVolume: The volume of the order in lots.

## Expert Initialization Function

The `OnInit()` function initializes necessary parameters for the Strategy Tester. It checks if the code is being run in the Strategy Tester and returns an error if not.

## Expert Start Function

The `OnTick()` function is the main function that gets executed on each tick of the market. It performs the following actions:

1. Checks if the Strategy Tester is running.
2. Checks if manual trade management is allowed.
3. Retrieves the current price.
4. Checks for buy and sell signals.
5. Calculates the entry price based on the stop loss.
6. Creates buy or sell orders.
7. Sets the stop loss and take profit levels for the orders.
8. Checks for manual position closure and order cancellation.

## Trade and Signal Functions

The code includes several functions that are responsible for checking trading conditions and signals. These functions include:

- `IsTradeAllowed()`: Checks if trading is allowed based on trading days and hours.
- `BuySignal()`: Implements the buy signal logic.
- `SellSignal()`: Implements the sell signal logic.
- `ClosePositionSignal()`: Implements the close position signal logic.
- `CancelOrderSignal()`: Implements the cancel order signal logic.

## Product Description

This code serves as a trading simulator in the MetaTrader 5 Strategy Tester. It allows traders to test and optimize their forex trading strategies before implementing them in live market conditions. The code includes features such as the ability to set stop loss and take profit levels, as well as manual trade management options. 

Please note that ForexRobotEasy is not the official developer of this product. We are only showcasing a sample code that can work as described in this product. To find the official developer of this product, please refer to MQL5. 

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/review-trading-simulator-in-strategytester-optimize-forex-strategies/).
