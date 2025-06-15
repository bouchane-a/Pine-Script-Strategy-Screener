# Pine Script Strategy Screener

## Overview

This Pine Script project provides a basic framework for screening multiple trading symbols simultaneously, designed to empower traders and developers to implement their own custom algorithms and strategies. It demonstrates how to fetch OHLC (Open, High, Low, Close) data for a predefined list of cryptocurrency pairs from Binance or other compatible data sources. **The simple bar-state-change detection strategy included serves as an example to illustrate how the script processes data and triggers events.** The core functionality revolves around the `STRATEGY` type, which processes market data and can be extended to apply various algorithms, with results displayed in a customizable table directly on your TradingView chart.

A [demo video](###demo) is available to see the script in action.

### Features

- ✅ Fetches OHLC data from multiple cryptocurrency symbols (e.g., BTCUSDT, ETHUSDT) on a specified exchange (Binance) or other compatible data sources.
- ✅ Defines a custom data type (`STRATEGY`) to encapsulate symbol-specific data and strategy logic.
- ✅ Detects new bars and updates bar state (bullish/bearish).
- ✅ Implements a simple strategy to identify bullish or bearish bar changes.
- ✅ Displays a real-time table on the chart showing symbol names, bar timestamps, and strategy event signals (e.g., "Bullish Bar", "Bearish Bar").
- ✅ Designed for concurrent data processing of multiple assets within Pine Script.
- ✅ Note on `request.*()` function limits: A script can use up to 40 unique calls to functions in the `request.*()` namespace, or up to 64 unique calls with a Professional plan.

### Requirements

A free or paid TradingView account is required to use this script.

### Getting Started

Copy the code from the `pinescript_strategy_screener.txt` file and paste it into your Pine Editor on TradingView. Save and add it to your chart.

The script will:
1.  Initialize a table on the bottom right of your chart.
2.  Fetch 1-minute OHLC data for the predefined list of cryptocurrency symbols from Binance (or the configured data source).
3.  For each symbol, it will analyze the previous bar to detect if a specific price action pattern (a bar changing from bearish to bullish, or bullish to bearish) has occurred.
4.  Continuously update the table, showing the symbol name, the timestamp of the last processed bar, and indicating if a "Bullish Bar" or "Bearish Bar" event was detected for that symbol.

### Demo



### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Contact

For questions or suggestions, please contact `bouchane.dev@gmail.com`.