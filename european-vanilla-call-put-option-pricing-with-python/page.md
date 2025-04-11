---
title: "European Vanilla Call and Put Option Pricing with Python"
description: Explore the intricate world of European Vanilla Call and Put Option Pricing with Python in algorithmic trading. This comprehensive guide investigates into fundamental options pricing principles and demonstrates how Python's robust libraries facilitate the development and integration of sophisticated financial models, essential for optimizing trading strategies. Discover best practices for precise options pricing and enhance your algorithmic trading efficiency using Python's vast ecosystem.
---


![Image](images/1.jpeg)

## Table of Contents

## What is a European Vanilla Call Option?

A European Vanilla Call Option is a type of financial contract that gives the buyer the right, but not the obligation, to buy a specific asset at a set price on a specific date in the future. The asset is usually a stock, but it can also be other things like commodities or currencies. The set price is called the strike price, and the specific date is known as the expiration date. This option is called "European" because it can only be exercised on the expiration date, not before.

The value of a European Vanilla Call Option depends on several factors, including the current price of the asset, the strike price, the time until the expiration date, and the expected volatility of the asset's price. If the asset's price is higher than the strike price at expiration, the option is "in the money," and the buyer can buy the asset at the lower strike price, then sell it at the higher market price to make a profit. If the asset's price is lower than the strike price at expiration, the option is "out of the money," and the buyer would not exercise the option, as it would result in a loss.

## What is a European Vanilla Put Option?

A European Vanilla Put Option is a financial contract that gives the buyer the right, but not the obligation, to sell a specific asset at a set price on a specific date in the future. This type of option is called "European" because it can only be exercised on the expiration date, not before. The asset can be a stock, commodity, or currency, and the set price is known as the strike price.

The value of a European Vanilla Put Option depends on factors like the current price of the asset, the strike price, the time until the expiration date, and how much the asset's price is expected to change. If the asset's price is lower than the strike price at expiration, the option is "in the money." This means the buyer can buy the asset at the lower market price and then sell it at the higher strike price to make a profit. If the asset's price is higher than the strike price at expiration, the option is "out of the money," and the buyer would not exercise the option, as it would result in a loss.

## How do European Vanilla Options differ from American Options?

European Vanilla Options and American Options are both types of financial contracts, but they have one main difference. European Options can only be used on the expiration date. This means you can only buy or sell the asset on that specific date. American Options, on the other hand, can be used at any time up to and including the expiration date. This gives the buyer more flexibility because they can choose the best time to use the option.

This difference affects how people use these options. With a European Option, you have to wait until the end to see if it's worth using. This can be good if you want to plan ahead and know exactly when you'll need to make a decision. With an American Option, you can act quickly if the market changes in your favor. This can be useful if you want to take advantage of good opportunities as soon as they come up. Both types of options have their own benefits, depending on what you need.

## What are the key components needed to price a European Vanilla Option?

To price a European Vanilla Option, you need to know a few important things. The first is the current price of the asset, like a stock or commodity, that the option is based on. Then, you need to know the strike price, which is the price at which you can buy or sell the asset if you use the option. The expiration date is also crucial because it tells you when the option can be used. Lastly, you need to consider the risk-free interest rate, which is the return you could get from a safe investment like a government bond.

Another key component is the expected volatility of the asset's price, which means how much the price might change over time. This is important because the more the price might change, the more valuable the option could be. To calculate the option's price, you can use a mathematical model like the Black-Scholes formula, which takes all these factors into account. By knowing these components, you can figure out how much the option is worth and decide if it's a good investment for you.

## What is the Black-Scholes model and how is it used for option pricing?

The Black-Scholes model is a mathematical formula that helps figure out the price of options, like European Vanilla Call and Put Options. It was created by economists Fischer Black and Myron Scholes in the early 1970s. The model uses several key pieces of information to come up with a price, including the current price of the asset, the strike price, the time until the option expires, the risk-free interest rate, and the expected volatility of the asset's price. By plugging these numbers into the Black-Scholes formula, you can get an estimate of what the option should be worth.

People use the Black-Scholes model because it helps them make better decisions about buying and selling options. For example, if you're thinking about buying a call option, you can use the model to see if the price seems fair based on the current market conditions. The model is especially helpful for European options, which can only be used on the expiration date. While the Black-Scholes model is very useful, it's not perfect. It makes some assumptions that don't always hold true in real life, like assuming that the asset's price follows a log-normal distribution and that there are no transaction costs. Despite these limitations, the Black-Scholes model remains a fundamental tool in the world of finance for pricing options.

## How can you calculate the price of a European Call Option using the Black-Scholes formula?

To calculate the price of a European Call Option using the Black-Scholes formula, you need to know five main things: the current price of the stock (S), the strike price (K), the time until the option expires (T), the risk-free interest rate (r), and the expected volatility of the stock's price (σ). The formula itself looks a bit complicated, but it helps you figure out how much the option should be worth. The formula is: C = S * N(d1) - K * e^(-rT) * N(d2), where C is the call option price, and N(d1) and N(d2) are values from a special table called the cumulative standard normal distribution. The values of d1 and d2 are calculated using the formula: d1 = (ln(S/K) + (r + σ^2/2) * T) / (σ * sqrt(T)) and d2 = d1 - σ * sqrt(T).

Using the Black-Scholes formula, you can plug in the numbers for S, K, T, r, and σ to find out what the call option should cost. For example, if the current stock price is $100, the strike price is $105, the option expires in 6 months (or 0.5 years), the risk-free interest rate is 5% (or 0.05), and the expected volatility is 20% (or 0.20), you can use these numbers in the formula to get the price of the call option. This helps you decide if buying the option is a good idea, based on what you think the stock price will do in the future. The Black-Scholes model gives you a fair estimate, but remember, it's not perfect because it makes some assumptions that might not always be true in real life.

## How can you calculate the price of a European Put Option using the Black-Scholes formula?

To calculate the price of a European Put Option using the Black-Scholes formula, you need to know the current price of the stock (S), the strike price (K), the time until the option expires (T), the risk-free interest rate (r), and the expected volatility of the stock's price (σ). The formula for a put option is: P = K * e^(-rT) * N(-d2) - S * N(-d1), where P is the put option price, and N(-d1) and N(-d2) are values from the cumulative standard normal distribution. The values of d1 and d2 are calculated the same way as for a call option: d1 = (ln(S/K) + (r + σ^2/2) * T) / (σ * sqrt(T)) and d2 = d1 - σ * sqrt(T).

Using this formula, you can plug in the numbers for S, K, T, r, and σ to find out what the put option should cost. For example, if the current stock price is $100, the strike price is $95, the option expires in 6 months (or 0.5 years), the risk-free interest rate is 5% (or 0.05), and the expected volatility is 20% (or 0.20), you can use these numbers in the formula to get the price of the put option. This helps you decide if buying the put option is a good idea, based on what you think the stock price will do in the future. The Black-Scholes model gives you a fair estimate, but remember, it's not perfect because it makes some assumptions that might not always be true in real life.

## What Python libraries are commonly used for option pricing?

When it comes to option pricing in Python, there are a few libraries that people often use. One of the most popular is NumPy, which is great for doing math and working with numbers. It helps with the calculations needed for models like Black-Scholes. Another useful library is SciPy, which has tools for statistics and optimization. It can help you find values from the standard normal distribution, which is important for the Black-Scholes formula.

There's also a library called QuantLib, which is made just for financial calculations. It has a lot of built-in functions for pricing different types of options, including European options. QuantLib is really helpful if you want to do more complex financial analysis. Lastly, some people use Pandas for handling data. It's good for organizing and analyzing information about stocks and options. These libraries together make it easier to price options and understand how they work.

## How can you implement the Black-Scholes model in Python to price a European Vanilla Call Option?

To price a European Vanilla Call Option using the Black-Scholes model in Python, you'll need to use libraries like NumPy and SciPy. First, you import these libraries and define the variables you need, like the current stock price, the strike price, the time to expiration, the risk-free interest rate, and the expected volatility. Then, you calculate the values of d1 and d2 using the formulas: d1 = (ln(S/K) + (r + σ^2/2) * T) / (σ * sqrt(T)) and d2 = d1 - σ * sqrt(T). After that, you use the cumulative standard normal distribution function from SciPy to find N(d1) and N(d2). Finally, you plug these values into the Black-Scholes formula for a call option: C = S * N(d1) - K * e^(-rT) * N(d2). This gives you the price of the call option.

Here's a simple example of how you might do this in Python. You'd start by importing NumPy and SciPy, then set up your variables. For instance, if the current stock price is $100, the strike price is $105, the time to expiration is 0.5 years, the risk-free interest rate is 0.05, and the expected volatility is 0.20, you'd calculate d1 and d2 using those numbers. Then, you'd use SciPy's norm.cdf function to find N(d1) and N(d2). Finally, you'd use the Black-Scholes formula to get the price of the call option. This way, you can see if it's a good deal to buy the option based on what you think the stock price will do in the future.

## How can you implement the Black-Scholes model in Python to price a European Vanilla Put Option?

To price a European Vanilla Put Option using the Black-Scholes model in Python, you start by importing the necessary libraries like NumPy and SciPy. You then define the key variables you need, such as the current stock price, the strike price, the time until the option expires, the risk-free interest rate, and the expected volatility of the stock's price. For example, if the stock price is $100, the strike price is $95, the time to expiration is 0.5 years, the risk-free interest rate is 5% (or 0.05), and the expected volatility is 20% (or 0.20), you can use these numbers in the Black-Scholes formula for a put option.

Next, you calculate the values of d1 and d2 using the formulas: d1 = (ln(S/K) + (r + σ^2/2) * T) / (σ * sqrt(T)) and d2 = d1 - σ * sqrt(T). After that, you use SciPy's norm.cdf function to find the values of N(-d1) and N(-d2) from the cumulative standard normal distribution. Finally, you plug these values into the Black-Scholes formula for a put option: P = K * e^(-rT) * N(-d2) - S * N(-d1). This gives you the price of the put option, helping you decide if it's a good idea to buy it based on what you think the stock price will do in the future.

## What are some common risk measures like Delta, Gamma, Theta, and Vega, and how can you calculate them for European Vanilla Options in Python?

Delta, Gamma, Theta, and Vega are important risk measures that help you understand how the price of an option might change. Delta tells you how much the option's price will change if the stock price changes by $1. For a European Vanilla Call Option, Delta is the value of N(d1) from the Black-Scholes formula. For a Put Option, Delta is N(d1) minus 1. Gamma measures how much Delta changes when the stock price changes by $1. It's the same for both Call and Put Options and is calculated as N'(d1) / (S * σ * sqrt(T)), where N'(d1) is the probability density function of the standard normal distribution.

Theta shows how much the option's price changes as time passes. For a Call Option, Theta is calculated as - (S * σ * N'(d1)) / (2 * sqrt(T)) - r * K * e^(-rT) * N(d2). For a Put Option, it's - (S * σ * N'(d1)) / (2 * sqrt(T)) + r * K * e^(-rT) * N(-d2). Vega measures how much the option's price changes when the volatility changes by 1%. It's the same for both Call and Put Options and is calculated as S * sqrt(T) * N'(d1). To calculate these in Python, you use the same variables and formulas as you do for pricing the options, but you focus on these specific parts of the Black-Scholes model.

## How can you validate the accuracy of your Python implementation of the Black-Scholes model for European Vanilla Options?

To make sure your Python code for the Black-Scholes model is correct, you can compare the prices it gives with prices from other sources. You might use prices from financial websites or other pricing models. If your code's prices are close to these other prices, it's a good sign that your code is working right. Another way to check is to use test cases where you already know the correct answer. For example, if you know that a call option with certain numbers should cost $5, you can put those numbers into your code and see if it gives you $5. If it does, that's another good sign.

You can also try changing the numbers you use in the model and see if the prices change in the way you expect. For example, if you increase the stock price, the price of a call option should go up, and the price of a put option should go down. If your code shows these changes, it's likely working correctly. Finally, you can look at the code itself to make sure you've used the right formulas and haven't made any mistakes. By using all these methods together, you can feel confident that your Python code for the Black-Scholes model is accurate.

## What is Understanding Options Pricing?

Options are financial derivatives that provide buyers the right, but not the obligation, to buy or sell an underlying asset at a specified price before a certain date. Understanding options and their pricing mechanisms is essential for traders who aim to develop effective trading strategies. Options play a pivotal role in financial markets by offering flexibility and opportunities for hedging, speculation, and enhancing investment returns.

Options pricing is a critical element in trading strategies as it determines the fair value of an option. The price of an option is typically influenced by factors such as the underlying asset's price, strike price, time to expiration, [volatility](/wiki/volatility-trading-strategies), [interest rate](/wiki/interest-rate-trading-strategies), and dividends. Accurate options pricing allows traders to make informed decisions by evaluating the potential risks and rewards associated with options trades.

Several key models exist for options pricing, with the Black-Scholes model being one of the most widely used. Introduced by Fischer Black, Myron Scholes, and Robert Merton in 1973, the Black-Scholes model provides a mathematical framework for pricing European-style options. The Black-Scholes formula for a call option is expressed as:

$$
C = S_0 N(d_1) - X e^{-rT} N(d_2)
$$

where:
- $C$ is the call option price.
- $S_0$ is the current stock price.
- $X$ is the strike price.
- $T$ is the time to expiration.
- $r$ is the risk-free interest rate.
- $N(d)$ is the cumulative distribution function of the standard normal distribution.
- $d_1 = \frac{\ln(S_0/X) + (r + \sigma^2/2)T}{\sigma\sqrt{T}}$
- $d_2 = d_1 - \sigma\sqrt{T}$
- $\sigma$ is the volatility of the stock.

Another popular model, the Binomial options pricing model, uses a discrete-time framework to model the underlying asset price over time. It considers multiple possible future paths that the stock price might follow and calculates the option price by working backward from the expiration date to the present. The model's flexibility allows it to handle a variety of conditions and types of options which the Black-Scholes model cannot, such as American options.

Monte Carlo simulations are also used for pricing options, particularly when dealing with complex derivative structures. This method involves simulating a large number of possible paths for the underlying asset price and averaging the payoffs to estimate the option's price. This stochastic technique is very powerful, although it can be computationally intensive.

Accurate pricing of options is crucial for traders to develop strategies that effectively balance risk and return. Mispricing can lead to inefficient trades and potential losses. Moreover, options pricing models must continually adapt to incorporate market changes and updated assumptions, such as shifts in volatility or interest rates.

Challenges in traditional options pricing approaches include assumptions of constant volatility and interest rates, which may not hold in real-world market conditions. Models like Black-Scholes also assume efficient markets and no dividends or transaction costs, which can oversimplify market realities. To address these challenges, traders and analysts often modify existing models or implement more sophisticated techniques to achieve more accurate and reliable pricing.

## How can you implement options pricing models in Python?

Implementing options pricing models using Python involves a combination of mathematical concepts and programming skills. Python's rich libraries and user-friendly syntax make it an ideal choice for this purpose. Here, we outline the implementation of several key options pricing models using Python, showcasing both the critical mathematical elements and the practical code snippets needed for execution.

### Black-Scholes Model

The Black-Scholes model is a cornerstone in options pricing. It's primarily used for pricing European options and involves the following formula for a call option:

$$
C = S_0 \Phi(d_1) - Xe^{-rt} \Phi(d_2)
$$

Where:
- $S_0$ is the current stock price
- $X$ is the strike price
- $r$ is the risk-free interest rate
- $t$ is the time to expiration
- $\Phi$ is the cumulative distribution function of the standard normal distribution
- $d_1 = \frac{\ln(S_0/X) + (r + \sigma^2/2)t}{\sigma\sqrt{t}}$
- $d_2 = d_1 - \sigma\sqrt{t}$

Here's how you can implement this in Python:

```python
import numpy as np
from scipy.stats import norm

def black_scholes_call(S, X, t, r, sigma):
    d1 = (np.log(S / X) + (r + 0.5 * sigma**2) * t) / (sigma * np.sqrt(t))
    d2 = d1 - sigma * np.sqrt(t)
    call = S * norm.cdf(d1) - X * np.exp(-r * t) * norm.cdf(d2)
    return call

# Example usage
S = 100  # Current stock price
X = 105  # Strike price
t = 1    # Time to expiration (in years)
r = 0.05 # Risk-free interest rate
sigma = 0.2  # Volatility

call_price = black_scholes_call(S, X, t, r, sigma)
print(f"Call option price: {call_price:.2f}")
```

### Binomial Options Pricing Model

The Binomial model offers a more flexible approach, especially for American options. It involves simulating possible paths the stock price might take and calculating option values at expiration back to the present. Here’s a simplified Python function for a binomial tree:

```python
def binomial_option_pricing(S, X, t, r, sigma, n, option_type='call'):
    dt = t / n
    u = np.exp(sigma * np.sqrt(dt))
    d = 1 / u
    p = (np.exp(r * dt) - d) / (u - d)

    option_price = np.zeros((n+1, n+1))

    for i in range(n+1):
        option_price[i, n] = max(0, (S * (u**i) * (d**(n-i)) - X) if option_type == 'call' else (X - S * (u**i) * (d**(n-i))))

    for j in range(n-1, -1, -1):
        for i in range(j+1):
            option_price[i, j] = np.exp(-r*dt) * (p * option_price[i+1, j+1] + (1-p) * option_price[i, j+1])

    return option_price[0, 0]

# Example usage
binomial_price = binomial_option_pricing(S, X, t, r, sigma, 100)
print(f"Binomial option price: {binomial_price:.2f}")
```

### QuantLib for Advanced Pricing

QuantLib is a comprehensive library for quantitative finance, providing advanced tools for options pricing and analysis. To use QuantLib in Python, you need to first install it:

```bash
pip install QuantLib-Python
```

QuantLib can be used to model complex derivatives and adjust the Black-Scholes model for dividend-paying stocks, interest rate models, etc.:

```python
import QuantLib as ql

def quantlib_black_scholes(S, X, t, r, sigma, option_type='Call'):
    maturity_date = ql.Date().todaysDate() + int(t * 360)
    spot_handle = ql.QuoteHandle(ql.SimpleQuote(S))
    flat_ts = ql.YieldTermStructureHandle(ql.FlatForward(0, ql.NullCalendar(), ql.QuoteHandle(ql.SimpleQuote(r)), ql.Actual360()))
    flat_vol_ts = ql.BlackVolTermStructureHandle(ql.BlackConstantVol(0, ql.NullCalendar(), ql.QuoteHandle(ql.SimpleQuote(sigma)), ql.Actual360()))

    payoff = ql.PlainVanillaPayoff(ql.Option.Call if option_type == 'call' else ql.Option.Put, X)
    exercise = ql.EuropeanExercise(maturity_date)

    process = ql.BlackScholesProcess(spot_handle, flat_ts, flat_vol_ts)
    option = ql.EuropeanOption(payoff, exercise)
    option.setPricingEngine(ql.AnalyticEuropeanEngine(process))

    price = option.NPV()
    return price

quantlib_price = quantlib_black_scholes(S, X, t, r, sigma)
print(f"QuantLib Black-Scholes price: {quantlib_price:.2f}")
```

### Monte Carlo Simulations

Monte Carlo simulations allow for modeling the stochastic nature of stock prices over time. These simulations involve generating numerous random price paths and averaging the payoff of the option over these paths:

```python
def monte_carlo_option_pricing(S, X, t, r, sigma, iterations):
    np.random.seed(0)
    payoff_sum = 0
    for _ in range(iterations):
        final_price = S * np.exp((r - 0.5 * sigma**2) * t + sigma * np.sqrt(t) * np.random.normal())
        payoff = max(0, final_price - X)
        payoff_sum += np.exp(-r * t) * payoff

    return payoff_sum / iterations

monte_carlo_price = monte_carlo_option_pricing(S, X, t, r, sigma, 10000)
print(f"Monte Carlo option price: {monte_carlo_price:.2f}")
```

### Data Visualization

Python libraries such as Matplotlib and Seaborn can visualize the results from these models, aiding in better decision-making:

```python
import matplotlib.pyplot as plt
import seaborn as sns

# Example data visualization
sns.set(style="whitegrid")
prices = [black_scholes_call(S, X, i/100, r, sigma) for i in range(1, 101)]
plt.plot(prices, label='Black-Scholes Prices')
plt.xlabel('Time to Expiry (in hundredths of years)')
plt.ylabel('Option Price')
plt.title('Options Pricing using Black-Scholes Model')
plt.legend()
plt.show()
```

By integrating these computational approaches with Python, traders can derive efficient and accurate options prices, forming a solid foundation for algorithmic trading strategies.

## How can options pricing be integrated into algo trading strategies?

Incorporating options pricing into algorithmic trading strategies enhances the ability to make accurate predictions and informed trading decisions. Accurate options pricing empowers traders to optimize their strategies by providing real-time insights into market conditions and potential price movements. This section explores how to effectively integrate options pricing into algorithmic trading strategies, highlighting strategic benefits, backtesting techniques, handling real-time data, and tools for deploying Python-based systems.

### Incorporating Options Pricing into Trading Strategies

Options pricing models provide crucial data on an option's theoretical value, considering factors such as the underlying asset price, strike price, time to expiration, volatility, and risk-free interest rate. Integrating these models allows traders to apply formulas like the Black-Scholes model, given by:

$$
C = S_0N(d_1) - Xe^{-rT}N(d_2)
$$

where $C$ is the call option price, $S_0$ is the present stock price, $X$ is the strike price, $r$ is the risk-free interest rate, $T$ is the time to maturity, and $N(d)$ is the cumulative distribution function of the standard normal distribution.

This formula facilitates strategies like delta-neutral trading, where traders hedge to reduce risk exposure, or volatility [arbitrage](/wiki/arbitrage), where opportunities arise from options mispricing relative to actual market volatility.

### Backtesting and Optimizing Strategies Using Python

Backtesting validates trading strategies by simulating historical data scenarios. Python's robust libraries, such as Pandas and Backtrader, allow for efficient backtesting. An example of a backtesting script using Backtrader might include:

```python
import backtrader as bt

class MyStrategy(bt.Strategy):
    def __init__(self):
        self.sma = bt.indicators.SimpleMovingAverage(period=15)

    def next(self):
        if self.sma > self.data.close:
            self.sell()
        elif self.sma < self.data.close:
            self.buy()

cerebro = bt.Cerebro()
cerebro.addstrategy(MyStrategy)

data = bt.feeds.YahooFinanceData(dataname='AAPL', fromdate='2020-01-01', todate='2021-01-01')
cerebro.adddata(data)
cerebro.run()
```

Optimizing strategies involves analyzing different parameters to maximize returns, fine-tuning entry and [exit](/wiki/exit-strategy) rules, and assessing the impact of varying levels of risk exposure. This process is crucial for adapting to evolving market environments.

### Handling Real-Time Data and Execution

Incorporating real-time data involves leveraging APIs and data feeds to ensure timely information processing. Python offers libraries like Alpaca, [Interactive Brokers](/wiki/interactive-brokers-api) API, and WebSocket to manage such data. A crucial aspect is ensuring low-latency execution by integrating Python with platforms designed to execute trading algorithms swiftly, ensuring that trading strategies respond effectively to market fluctuations.

### Tools and Platforms for Deployment

Deploying robust algorithmic trading systems necessitates using platforms that support scalability and performance. Python-centric platforms such as QuantConnect and Zipline offer extensive infrastructure for developing, backtesting, and executing algorithms. They provide cloud-based setups, reducing the need for personal server maintenance while offering extensive community support and data resources.

Additionally, employing the right tools for monitoring and logging ensures transparency and allows for swift troubleshooting and strategy adjustments. Platforms like Docker and Jenkins facilitate continuous integration and deployment, enhancing the reliability of trading systems.

In summary, integrating options pricing models using Python enriches algorithmic trading strategies by providing data-driven insights and facilitating robust system deployment. Accurate backtesting and seamless real-time execution are critical to developing successful trading models capable of navigating complex financial markets.

## References & Further Reading

[1]: Black, F., & Scholes, M. (1973). ["The Pricing of Options and Corporate Liabilities."](https://www.cs.princeton.edu/courses/archive/fall09/cos323/papers/black_scholes73.pdf) The Journal of Political Economy, 81(3), 637-654.

[2]: Cox, J. C., Ross, S. A., & Rubinstein, M. (1979). ["Option Pricing: A Simplified Approach."](https://www.sciencedirect.com/science/article/pii/0304405X79900151) Journal of Financial Economics, 7(3), 229-263.

[3]: Boyle, P. P. (1977). ["Options: A Monte Carlo Approach."](https://www.sciencedirect.com/science/article/pii/0304405X77900058) Journal of Financial Economics, 4(3), 323-338.

[4]: Hull, J. C. (2017). ["Options, Futures, and Other Derivatives."](https://www.amazon.com/Options-Futures-Other-Derivatives-9th/dp/0133456315) 9th Edition, Pearson.

[5]: Wilmott, P. (2006). ["Paul Wilmott Introduces Quantitative Finance."](https://www.wiley.com/en-us/Paul+Wilmott+Introduces+Quantitative+Finance,+2nd+Edition-p-9781118836798) 2nd Edition, Wiley.

[6]: NumpPy Developers. ["NumPy: The fundamental package for scientific computing with Python."](https://github.com/numpy/numpy)

[7]: McKinney, W. (2010). ["Data Structures for Statistical Computing in Python."](http://conference.scipy.org.s3-website-us-east-1.amazonaws.com/proceedings/scipy2010/pdfs/mckinney.pdf) Proceedings of the 9th Python in Science Conference.

[8]: Pedregosa, F., Varoquaux, G., Gramfort, A., Michel, V., Thirion, B., Grisel, O., et al. (2011). ["Scikit-learn: Machine Learning in Python."](https://dl.acm.org/doi/10.5555/1953048.2078195) Journal of Machine Learning Research, 12, 2825-2830.

[9]: QuantLib. ["QuantLib: A free/open-source library for quantitative finance."](https://www.quantlib.org/)

[10]: Perez, F., & Granger, B. E. (2007). ["IPython: A System for Interactive Scientific Computing."](https://ieeexplore.ieee.org/document/4160251) Computing in Science & Engineering, 9(3), 21-29.