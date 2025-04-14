---
title: "Broken Wing Butterfly Options Trading Strategy in Python"
description: Discover the Broken Wing Butterfly options trading strategy in Python, an innovative technique for optimizing algorithmic trading outcomes. This advanced strategy enhances the traditional Butterfly Spread by generating net credit and offers an asymmetrical risk-reward profile, making it suitable for traders to exploit specific market conditions. Explore its setup, profitability potential, and risk management, providing valuable insights for incorporating this method into your algo trading practice for effectively navigating complex market landscapes.
---


![Image](images/1.png)

## Table of Contents

## What is a Broken Wing Butterfly options trading strategy?

A Broken Wing Butterfly is an options trading strategy that involves buying and selling options with different strike prices to create a position that can profit from a specific range of stock price movements. It's called "broken wing" because the distances between the strike prices are not equal, unlike a standard butterfly spread. This strategy is often used when a trader has a directional bias, expecting the stock to move towards one of the wings of the butterfly but not beyond it.

To set up a Broken Wing Butterfly, a trader typically buys an in-the-money option, sells two at-the-money options, and buys an out-of-the-money option. The goal is to profit if the stock price stays within a certain range at expiration. If the stock price moves towards the "broken wing" side, the strategy can still be profitable, but if it moves too far in that direction, the potential losses can be higher than with a standard butterfly. This strategy can be useful for traders who want to take advantage of a stock's expected movement while managing their risk.

## How does a Broken Wing Butterfly differ from a standard Butterfly spread?

A Broken Wing Butterfly and a standard Butterfly spread are both options trading strategies, but they have some key differences. In a standard Butterfly spread, the distances between the strike prices of the options are equal. For example, if you're using call options, you might buy one call at a lower strike price, sell two calls at a middle strike price, and buy one call at a higher strike price, with the same distance between each strike. This setup is designed to profit if the stock price stays close to the middle strike price at expiration.

In contrast, a Broken Wing Butterfly has unequal distances between the strike prices, which is where it gets its name. This means you might buy an in-the-money option, sell two at-the-money options, and buy an out-of-the-money option, but the distance between the lower and middle strikes is different from the distance between the middle and higher strikes. This setup allows for a directional bias, meaning you expect the stock to move towards one side but not too far. While a standard Butterfly is more about staying within a tight range, a Broken Wing Butterfly can still make money if the stock moves towards the "broken wing" side, but it also carries more risk if the stock moves too far in that direction.

## What are the key components needed to set up a Broken Wing Butterfly?

To set up a Broken Wing Butterfly, you need to buy and sell options with different strike prices. You start by buying an in-the-money option, which means it has a strike price that is favorable compared to the current stock price. Then, you sell two at-the-money options, which have a strike price close to the current stock price. Finally, you buy an out-of-the-money option, which has a strike price that is less favorable compared to the current stock price. The key is that the distances between these strike prices are not equal, which is what makes it a "broken wing" butterfly.

This setup allows you to make money if the stock price moves towards one side but not too far. For example, if you think the stock will go up a bit but not too much, you would set up the broken wing on the upside. The strategy can still be profitable if the stock moves towards the broken wing, but it also carries more risk if the stock moves too far in that direction. This is different from a standard butterfly spread, where the distances between the strike prices are equal and the goal is to keep the stock price within a tight range.

## Can you explain the payoff diagram for a Broken Wing Butterfly?

A payoff diagram for a Broken Wing Butterfly shows how much money you could make or lose depending on where the stock price ends up at expiration. Imagine a graph where the horizontal line shows different stock prices, and the vertical line shows how much money you make or lose. The diagram will have a shape that looks like a butterfly with one wing bigger than the other. If the stock price stays in the middle, you make the most money. As the stock price moves towards the bigger wing, you can still make money, but if it goes too far, you start to lose money. If the stock price moves towards the smaller wing, you lose money more quickly.

The key thing to remember is that the Broken Wing Butterfly is set up so that you can make money if the stock moves a bit in one direction but not too far. The bigger wing, or the "broken wing," is where you expect the stock to go. If it goes there and stays within a certain range, you can make money. But if it goes past the broken wing, you could lose more money than with a regular butterfly spread. This is because the distances between the strike prices are not equal, which makes the strategy more risky but also gives you a chance to make money if the stock moves in the direction you expect.

## What are the potential risks and rewards associated with this strategy?

The main reward of using a Broken Wing Butterfly is that it can make you money if the stock price moves a bit in the direction you expect but not too far. This is different from a regular butterfly spread because it gives you a chance to profit from a small move in the stock price. If the stock stays close to where you want it to be at expiration, you can make the most money. This strategy can be useful if you have a good idea of where the stock is going to go but you're not sure it will go all the way there.

The risks of a Broken Wing Butterfly are higher than with a regular butterfly spread because the distances between the strike prices are not equal. If the stock moves too far in the direction of the bigger wing, you could lose more money than you would with a regular butterfly. This is because the strategy is set up to make money if the stock moves towards the bigger wing but not past it. If the stock moves too far, you could end up losing money. It's important to understand these risks and to have a plan for what you'll do if the stock doesn't move the way you expect.

## How do you calculate the maximum profit and loss for a Broken Wing Butterfly?

To calculate the maximum profit for a Broken Wing Butterfly, you need to figure out the difference between the strike prices of the options and the net cost of setting up the trade. The maximum profit happens when the stock price is at the strike price of the options you sold, which is the middle strike price. You subtract the net cost of the trade from the difference between the strike prices of the options you bought and sold. For example, if you bought an in-the-money call at $90, sold two at-the-money calls at $100, and bought an out-of-the-money call at $110, and the net cost of the trade was $2, then the maximum profit would be the difference between $100 and $90 (which is $10) minus the $2 net cost, which equals $8 per share.

The maximum loss for a Broken Wing Butterfly depends on which direction the stock price moves. If the stock price goes above the highest strike price or below the lowest strike price, you could lose money. To find the maximum loss, you need to look at the worst-case scenario. If the stock price goes above the highest strike price, the maximum loss would be the net cost of the trade plus the difference between the highest and middle strike prices. If the stock price goes below the lowest strike price, the maximum loss would be the net cost of the trade. For example, using the same strikes as before, if the stock price goes above $110, the maximum loss would be $2 (the net cost) plus $10 (the difference between $110 and $100), which equals $12 per share. If the stock price goes below $90, the maximum loss would just be the $2 net cost of the trade.

## What market conditions are ideal for implementing a Broken Wing Butterfly?

The best time to use a Broken Wing Butterfly is when you think the stock will move a bit in one direction but not too far. This strategy works well if you expect the stock to go up or down a little but then stay in a certain range. For example, if you think a stock will go up a bit because of good news, but you don't think it will keep going up a lot, a Broken Wing Butterfly can help you make money from that small move.

Another good time to use this strategy is when the market is a bit unsure, but you have a good idea of where the stock might go. If you think the stock will move towards one side but not past it, a Broken Wing Butterfly can be a good choice. It's important to pick the right strike prices and to keep an eye on how the stock is moving, so you can adjust your strategy if you need to.

## How can you use Python to simulate a Broken Wing Butterfly strategy?

To simulate a Broken Wing Butterfly strategy using Python, you can use libraries like NumPy and Matplotlib to create a payoff diagram and calculate potential profits and losses. First, you would define the strike prices for your options: an in-the-money option, two at-the-money options, and an out-of-the-money option. You would also need to set the current stock price and the premiums for each option. Then, you can use NumPy to create an array of possible stock prices at expiration and calculate the payoff for each scenario. The payoff is calculated by adding the value of the in-the-money option, subtracting twice the value of the at-the-money options, and adding the value of the out-of-the-money option. Finally, you subtract the net cost of setting up the trade to get the profit or loss for each stock price.

Once you have the payoff calculations, you can use Matplotlib to plot the results. The x-axis of the plot would represent different stock prices at expiration, and the y-axis would show the profit or loss. The resulting graph will look like a butterfly with one wing bigger than the other, showing how the strategy can make money if the stock price moves towards the bigger wing but not too far. By adjusting the strike prices and premiums, you can see how different setups affect the potential outcomes of the Broken Wing Butterfly strategy. This simulation can help you understand the risks and rewards of the strategy before you use it in the real market.

## What Python libraries are essential for options trading analysis?

For options trading analysis, Python libraries like NumPy and Pandas are very important. NumPy helps you do math quickly, which is useful for figuring out things like the value of options at different stock prices. Pandas is great for working with data, so you can easily organize and look at information about your trades. These libraries make it easier to handle big sets of numbers and do calculations that are important for options trading.

Another useful library is Matplotlib, which helps you make graphs and charts. With Matplotlib, you can draw payoff diagrams to see how much money you might make or lose with different options strategies. This can help you understand the risks and rewards of your trades better. For more advanced options analysis, you might also use libraries like SciPy for statistical calculations and QuantLib for financial modeling. These libraries can help you with things like calculating option Greeks and simulating different market scenarios.

## Can you provide a Python code example to calculate the Greeks for a Broken Wing Butterfly?

To calculate the Greeks for a Broken Wing Butterfly using Python, we need to use libraries like NumPy and SciPy. The Greeks are important because they tell us how the value of our options changes with things like the stock price, time, and [volatility](/wiki/volatility-trading-strategies). We'll set up our Broken Wing Butterfly with four options: an in-the-money option, two at-the-money options, and an out-of-the-money option. We'll use the Black-Scholes model to calculate the value of each option and then combine them to find the total value of the Broken Wing Butterfly. Then, we can use the formulas for the Greeks to see how the value of our strategy changes with different factors.

Here's some simple Python code to do this. We'll use the `scipy.stats` module to get the cumulative distribution function (CDF) needed for the Black-Scholes model. We'll define our options with their strike prices, the current stock price, time to expiration, risk-free rate, and volatility. Then, we'll calculate the value of each option and combine them to get the total value of the Broken Wing Butterfly. After that, we'll use the formulas for Delta, Gamma, Theta, and Vega to see how our strategy reacts to changes in the stock price, time, and volatility. This code will give us a good idea of the risks and rewards of our Broken Wing Butterfly.

```python
import numpy as np
from scipy.stats import norm

# Define parameters
S = 100  # Current stock price
K1 = 90  # Strike price of the in-the-money option
K2 = 100  # Strike price of the at-the-money options
K3 = 110  # Strike price of the out-of-the-money option
T = 1  # Time to expiration (in years)
r = 0.05  # Risk-free rate
sigma = 0.2  # Volatility

# Black-Scholes formula for call option
def black_scholes_call(S, K, T, r, sigma):
    d1 = (np.log(S / K) + (r + 0.5 * sigma ** 2) * T) / (sigma * np.sqrt(T))
    d2 = d1 - sigma * np.sqrt(T)
    return S * norm.cdf(d1) - K * np.exp(-r * T) * norm.cdf(d2)

# Calculate option values
c1 = black_scholes_call(S, K1, T, r, sigma)
c2 = black_scholes_call(S, K2, T, r, sigma)
c3 = black_scholes_call(S, K3, T, r, sigma)

# Calculate Broken Wing Butterfly value
broken_wing_value = c1 - 2 * c2 + c3

# Calculate Greeks
# Delta
delta = (black_scholes_call(S + 0.01, K1, T, r, sigma) - black_scholes_call(S - 0.01, K1, T, r, sigma)) / 2 - 2 * (black_scholes_call(S + 0.01, K2, T, r, sigma) - black_scholes_call(S - 0.01, K2, T, r, sigma)) / 2 + (black_scholes_call(S + 0.01, K3, T, r, sigma) - black_scholes_call(S - 0.01, K3, T, r, sigma)) / 2

# Gamma
gamma = (black_scholes_call(S + 0.01, K1, T, r, sigma) - 2 * black_scholes_call(S, K1, T, r, sigma) + black_scholes_call(S - 0.01, K1, T, r, sigma)) / 0.01 ** 2 - 2 * (black_scholes_call(S + 0.01, K2, T, r, sigma) - 2 * black_scholes_call(S, K2, T, r, sigma) + black_scholes_call(S - 0.01, K2, T, r, sigma)) / 0.01 ** 2 + (black_scholes_call(S + 0.01, K3, T, r, sigma) - 2 * black_scholes_call(S, K3, T, r, sigma) + black_scholes_call(S - 0.01, K3, T, r, sigma)) / 0.01 ** 2

# Theta
theta = (black_scholes_call(S, K1, T - 1/365, r, sigma) - black_scholes_call(S, K1, T, r, sigma)) - 2 * (black_scholes_call(S, K2, T - 1/365, r, sigma) - black_scholes_call(S, K2, T, r, sigma)) + (black_scholes_call(S, K3, T - 1/365, r, sigma) - black_scholes_call(S, K3, T, r, sigma))

# Vega
vega = (black_scholes_call(S, K1, T, r, sigma + 0.01) - black_scholes_call(S, K1, T, r, sigma - 0.01)) / 2 - 2 * (black_scholes_call(S, K2, T, r, sigma + 0.01) - black_scholes_call(S, K2, T, r, sigma - 0.01)) / 2 + (black_scholes_call(S, K3, T, r, sigma + 0.01) - black_scholes_call(S, K3, T, r, sigma - 0.01)) / 2

print(f"Broken Wing Butterfly Value: {broken_wing_value}")
print(f"Delta: {delta}")
print(f"Gamma: {gamma}")
print(f"Theta: {theta}")
print(f"Vega: {vega}")
```

## How do you adjust a Broken Wing Butterfly position in response to market movements?

Adjusting a Broken Wing Butterfly position involves making changes to your options based on how the stock price is moving. If the stock is moving towards the bigger wing but not too far, you might not need to do anything because the strategy is working as planned. But if the stock starts moving too close to the bigger wing, you might want to roll up the short options to a higher strike price to reduce your risk. This means selling the options you sold before and buying them back at a higher price, then selling new options at an even higher strike price. This can help you keep making money if the stock keeps going up, but it costs more money to do this.

On the other hand, if the stock is moving towards the smaller wing, you might want to roll down the short options to a lower strike price. This means buying back the options you sold and selling new ones at a lower price. This can help you make money if the stock keeps going down, but it also costs money to make these changes. It's important to keep an eye on the stock and be ready to make these adjustments if things aren't going the way you expected. By making these changes, you can try to keep your Broken Wing Butterfly strategy working well even when the market moves.

## What advanced techniques can be applied to optimize a Broken Wing Butterfly strategy using Python?

To optimize a Broken Wing Butterfly strategy using Python, you can use advanced techniques like [backtesting](/wiki/backtesting) and Monte Carlo simulations. Backtesting involves running your strategy on historical data to see how it would have performed in the past. You can use Python to write a script that goes through old stock prices and calculates how much money you would have made or lost with different setups of your Broken Wing Butterfly. This helps you find the best strike prices and expiration dates to use. Monte Carlo simulations are another way to optimize your strategy. They involve running lots of different scenarios with random stock price movements to see how your strategy might do in the future. Python can help you do these simulations quickly and see how different changes to your strategy might affect your results.

Another advanced technique is to use [machine learning](/wiki/machine-learning) to predict stock price movements and adjust your Broken Wing Butterfly accordingly. You can use Python libraries like scikit-learn to build models that look at things like past stock prices, news, and other data to guess where the stock might go next. Then, you can use these predictions to choose the best strike prices for your options. This can help you make your strategy more profitable by being ready for different market conditions. By using these advanced techniques in Python, you can make your Broken Wing Butterfly strategy work better and be more prepared for what the market might do.

## What are the considerations for profitability and risk?

The profitability of the Broken Wing Butterfly strategy hinges on the position of the asset relative to the options' strike prices at expiration. To achieve maximum profit, the asset's price should ideally settle at the central strike price. In this scenario, the trader benefits from the premium collected initially (net credit) along with the difference between the strike prices of the purchased and sold options, thereby maximizing the profitability of the strategy. However, achieving the asset's expiration precisely at the central strike price is statistically uncommon, thus requiring careful strategic planning and execution.

The mathematical formulation for the maximum profit of a Broken Wing Butterfly strategy can be expressed as follows:

$$

\text{Max Profit} = \text{Width of the short spread} + \text{Net Credit Received} 
$$

Here, the width of the short spread refers to the difference in strike prices between the nearest option sold and the option purchased closer to the money. The net credit is the premium received by setting up the trade.

Conversely, the maximum loss occurs if the farthest option, often the "broken" wing, ends up being in-the-money at expiration. This situation leads to a loss calculated by:

$$

\text{Max Loss} = \text{Width of the wider spread} - \text{Net Credit Received} 
$$

This loss represents the financial risk a trader assumes if the asset price moves beyond the protective strike of the long options when the position reaches maturity.

Implementing the Broken Wing Butterfly demands meticulous evaluation of option pricing, implied volatility, and market conditions. Given that the probability of the desired price position at expiration is low, traders need to assess the likelihood of various price movements and set up scenarios in which the strategy's structure remains favorable. Risk management tools and strategic adjustments, such as rolling options closer to expiration or changing the strike arrangement, help mitigate potential downsides.

Ultimately, while the strategy holds potential for substantial gains with minimal initial capital outlay, it primarily functions as a sophisticated technique better suited for traders with substantial market understanding and experience in optimizing complex option structures.

## References & Further Reading

[1]: ["Option Volatility and Pricing: Advanced Trading Strategies and Techniques"](https://www.amazon.com/Option-Volatility-Pricing-Strategies-Techniques/dp/0071818774) by Sheldon Natenberg

[2]: ["Trading Options Greeks: How Time, Volatility, and Other Pricing Factors Drive Profits"](https://www.amazon.com/Trading-Options-Greeks-Volatility-Pricing/dp/1118133161) by Dan Passarelli

[3]: Haug, E. G. (2007). ["The Complete Guide to Option Pricing Formulas."](https://www.amazon.com/Complete-Guide-Option-Pricing-Formulas/dp/0786312408) McGraw-Hill.

[4]: Mitchell, M., & Burns, J. (2020). ["Python for Finance: Analyze Big Financial Data"](https://books.google.com/books/about/Python_for_Finance.html?id=E93SBQAAQBAJ) by Yves Hilpisch

[5]: ["Options, Futures, and Other Derivatives"](https://www.amazon.com/Options-Futures-Other-Derivatives-5th/dp/0130090565) by John C. Hull