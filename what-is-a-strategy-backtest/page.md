---
title: "What is a strategy backtest?"
description: "Discover the concept of a strategy backtest and its importance in assessing a trading strategy's viability using historical data. Learn the steps involved in conducting a backtest, including strategy definition, data acquisition, simulation, evaluation, analysis, and potential risks. Explore resources for further study and datasets to get started in quantitative trading."
---



A strategy backtest is a method of assessing the viability of a trading strategy by testing it on historical data. In other words, it simulates how a strategy would have performed had it been implemented in the past, in order to obtain an indication of its possible future performance.

Here are the main steps in a backtest:

1. **Strategy definition**: First, the trading strategy must be clearly defined, whether it's based on technical indicators, fundamental events, algorithms or other criteria.
2. **Data acquisition**: To carry out a backtest, it is necessary to have access to relevant historical data. This can include asset prices, trading volumes, and anything else relevant to the strategy.
3. **Simulation**: Using the historical data, the strategy is then "executed" retrospectively, as if trading in real time over the chosen historical period.
4. **Evaluation**: Once the simulation is complete, the strategy's performance is evaluated using various measures, such as return, volatility, Sharpe ratio, maximum drawdown, etc.
5. **Analysis**: After evaluation, it is essential to analyze the results to understand the strategy's strengths and weaknesses, and to see if it is viable or if adjustments are necessary.

> 

It is crucial to note that a good backtest result does not necessarily guarantee similar future performance. There is a risk of "over-optimization", where a strategy may be over-adapted to historical data and therefore not perform well in new or changing market conditions. It is always advisable to use backtesting as one tool among others in the process of deciding and evaluating a trading strategy.

💡 **Read more:**

- Trading strategies papers with code on [Equities](https://wiki.paperswithbacktest.com/trading-strategies/equities), [Cryptocurrencies](https://wiki.paperswithbacktest.com/trading-strategies/cryptocurrencies), [Commodities](https://wiki.paperswithbacktest.com/trading-strategies/commodities), [Currencies](https://wiki.paperswithbacktest.com/trading-strategies/currencies), [Bonds](https://wiki.paperswithbacktest.com/trading-strategies/bonds), [Options](https://wiki.paperswithbacktest.com/trading-strategies/options)
- [A curated list](https://github.com/paperswithbacktest/awesome-systematic-trading) of awesome libraries, packages, strategies, books, blogs, and tutorials for systematic trading
- [A bunch of datasets](https://huggingface.co/paperswithbacktest) for quantitative trading
- [A website to help you](https://paperswithbacktest.com/) become a quant trader and achieve financial independence