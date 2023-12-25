# Chart Local Time Indicator

This code is a custom indicator for MetaTrader 5 that displays the local time on the chart. It is provided as a sample code by Forex Robot Easy Team and can enhance forex trading by showing the local time of each candlestick.

## How it Works

The indicator uses the `OnInit()` function for initialization, `OnDeinit()` function for deinitialization, and `OnCalculate()` function for the main iteration process.

### Initialization

In the `OnInit()` function, the indicator buffer is mapped using `SetIndexBuffer()`, which assigns the buffer to the `TimeBuffer` array.

### Deinitialization

The `OnDeinit()` function is called when the indicator is removed from the chart or the terminal is closed. In this function, the `TimeBuffer` array is cleared using `ArrayInitialize()`.

### Iteration

The `OnCalculate()` function is called for each new tick or when the chart is scrolled. It receives various parameters such as `rates_total`, `prev_calculated`, and arrays representing time, open, high, low, close prices, tick volume, volume, and spread.

The main purpose of this function is to display the local time on the chart. It loops through the new bars since the last calculation (`prev_calculated`) and calculates the local time for each bar using `TimeLocal()` function. The calculated local time is then stored in the `TimeBuffer` array and printed using `Print()` function.

## Product Description

[Chart Local Time](https://forexroboteasy.com/forex-robot-review/chart-local-time-mt5-review-enhance-forex-trading-with-local-time-display/) is a custom indicator for MetaTrader 5 that enhances forex trading by displaying the local time on the chart. It is a powerful tool for traders who want to keep track of the time while analyzing price movements.

With Chart Local Time, traders can easily identify the time at which each candlestick is formed, allowing them to make more informed trading decisions based on the specific time of price action. This indicator eliminates the need to manually convert server time to local time, providing traders with a convenient and efficient solution.

Please note that Forex Robot Easy Team is not the official developer of this product. We are only showcasing a sample code that can work as described in this product. To find the official developer of this product, please refer to MQL5. For detailed reviews and trading results, visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/chart-local-time-mt5-review-enhance-forex-trading-with-local-time-display/).
