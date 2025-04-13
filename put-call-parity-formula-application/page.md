---
title: "Put-Call Parity: Formula and Application"
description: "Explore the concept of put-call parity and its applications in algorithmic trading Learn how this principle aids in identifying arbitrage opportunities and market equilibrium"
---


![Image](images/1.jpeg)

## Table of Contents

## What is Put-Call Parity?

Put-Call Parity is a principle in options pricing that shows the relationship between the prices of put options and call options of the same stock, with the same strike price and expiration date. It helps traders understand how these options should be priced relative to each other and to the underlying stock. The basic idea is that owning a call option (which gives you the right to buy a stock) and selling a put option (which gives someone else the right to sell you the stock) should be the same as just owning the stock itself.

In simple terms, the formula for Put-Call Parity is: the price of a call option plus the present value of the strike price equals the price of a put option plus the current stock price. If this equation doesn't hold, there might be an opportunity for arbitrage, where traders can make a risk-free profit by exploiting the price difference. This principle is important for ensuring that options markets remain efficient and that the prices of options reflect their true value based on the underlying stock.

## What are the basic components of the Put-Call Parity formula?

The Put-Call Parity formula has four main parts: the price of a call option, the price of a put option, the current stock price, and the present value of the strike price. The call option gives you the right to buy the stock at the strike price before the option expires. The put option gives you the right to sell the stock at the strike price before it expires. The current stock price is what the stock is trading for right now. The present value of the strike price is what the strike price would be worth today, considering the time value of money.

The formula says that the price of a call option plus the present value of the strike price should equal the price of a put option plus the current stock price. If this balance doesn't hold, there might be a chance for arbitrage, which means making a profit without taking any risk. This relationship helps keep the options market fair and makes sure that the prices of options make sense compared to the stock they are based on.

## How does Put-Call Parity relate to options pricing?

Put-Call Parity is a key idea in options pricing because it shows how the prices of put and call options should be connected. It says that if you have a call option and sell a put option with the same strike price and expiration date, it should be the same as just owning the stock itself. This relationship helps traders understand what the prices of options should be based on the current stock price and the time value of money. If the prices don't match up, it might mean there's a chance to make a risk-free profit by buying and selling the right options and stocks.

This principle is important for keeping the options market fair. If the prices of puts and calls get out of balance, traders can use arbitrage to bring them back in line. This means they can buy and sell options and stocks in a way that makes a profit without taking any risk. By doing this, they help make sure that the prices of options stay correct and reflect the true value of the underlying stock. So, Put-Call Parity is a tool that helps traders and keeps the market working smoothly.

## Can you explain the Put-Call Parity formula?

Put-Call Parity is like a balance rule for options. It says that the price of a call option plus the present value of the strike price should equal the price of a put option plus the current stock price. A call option lets you buy a stock at a certain price, called the strike price, before the option expires. A put option lets you sell a stock at the strike price before it expires. The present value of the strike price is what that strike price would be worth today if you account for the time value of money. So, if you add the price of a call option and the present value of the strike price, it should be the same as adding the price of a put option and the current stock price.

If this balance doesn't hold true, there might be a chance for arbitrage. Arbitrage means you can make a profit without taking any risk by buying and selling the right options and stocks. For example, if the call option is too cheap or the put option is too expensive, you could buy the call, sell the put, and buy the stock to make a risk-free profit. This helps keep the options market fair and makes sure that the prices of options make sense compared to the stock they are based on. Put-Call Parity is a tool that traders use to check if option prices are correct and to find opportunities to make money.

## What assumptions are made in the Put-Call Parity model?

The Put-Call Parity model makes some important assumptions to keep things simple. It assumes that there are no transaction costs when you buy or sell options or stocks. It also assumes that you can borrow or lend money at the same interest rate, which is called the risk-free rate. This means you can buy and sell without worrying about extra fees or different interest rates messing up the balance.

Another big assumption is that the options and stocks can be bought and sold in any amount you want, which is called perfect divisibility. This means you can always find someone to trade with, no matter how much you want to buy or sell. The model also assumes that there are no risks of the company going bankrupt or other big changes happening to the stock. These assumptions help make the math easier and keep the focus on how the prices of puts and calls should relate to each other and the stock price.

## How can Put-Call Parity be used to identify arbitrage opportunities?

Put-Call Parity can help traders find arbitrage opportunities by showing when the prices of options and stocks don't match up like they should. If the price of a call option plus the present value of the strike price doesn't equal the price of a put option plus the current stock price, there might be a chance to make a risk-free profit. For example, if the call option is too cheap compared to the put option and the stock, a trader could buy the call option, sell the put option, and buy the stock. By doing this, they can lock in a profit without taking any risk, because the prices are out of balance.

This kind of arbitrage helps keep the options market fair. When traders spot these opportunities and act on them, they push the prices back into line with what the Put-Call Parity formula says they should be. This means that if the call option is too cheap, buying it will make its price go up. If the put option is too expensive, selling it will make its price go down. Over time, this action by traders helps make sure that the prices of options stay correct and reflect the true value of the underlying stock.

## What are the limitations of Put-Call Parity in real-world trading?

In real-world trading, Put-Call Parity has some limitations because it makes assumptions that don't always hold true. One big assumption is that there are no transaction costs. But in real life, every time you buy or sell options or stocks, you have to pay fees. These fees can add up and change how much money you can make from arbitrage. Another assumption is that you can borrow or lend money at the same interest rate, called the risk-free rate. But in reality, interest rates can be different depending on who you are and how much you want to borrow or lend. This can make the math more complicated and affect whether you can make a risk-free profit.

Another limitation is that Put-Call Parity assumes you can buy and sell any amount of options or stocks you want, but in real life, there can be limits on how much you can trade. Also, the model doesn't take into account things like the company going bankrupt or other big changes that can affect the stock price. These risks can make the prices of options move in ways that the model doesn't predict. So, while Put-Call Parity is a useful tool for understanding how options should be priced, traders need to be careful and consider these real-world factors when using it to find arbitrage opportunities.

## How does Put-Call Parity apply to American options versus European options?

Put-Call Parity works differently for American options compared to European options because of when you can use them. With European options, you can only use them on the day they expire. This makes the math easier because you know exactly when you'll use the option. So, the Put-Call Parity formula for European options is simple: the price of a call option plus the present value of the strike price equals the price of a put option plus the current stock price. If this balance doesn't hold, there might be a chance to make a risk-free profit by buying and selling the right options and stocks.

For American options, things get more complicated because you can use them any time before they expire. This early use option means the prices of American options can be different from European options. The Put-Call Parity for American options still says that the price of a call option plus the present value of the strike price should equal the price of a put option plus the current stock price, but you have to think about the chance that someone might use the option early. This makes it harder to find arbitrage opportunities because you have to consider how early use might affect the prices. So, while the basic idea of Put-Call Parity is the same for both types of options, it's trickier to use with American options.

## Can you provide an example of how to use Put-Call Parity to check for mispricing in options?

Let's say you want to check if the prices of options for a stock are right. You look at a stock that's trading at $50 right now. There's a call option for this stock with a strike price of $50 that costs $3, and a put option with the same strike price that costs $2. The option will expire in one year, and the risk-free interest rate is 5%. To use Put-Call Parity, you need to find the present value of the strike price. The present value of $50 one year from now at a 5% interest rate is about $47.62. According to Put-Call Parity, the price of the call option ($3) plus the present value of the strike price ($47.62) should equal the price of the put option ($2) plus the current stock price ($50). So, $3 + $47.62 = $50.62, and $2 + $50 = $52. Since $50.62 is less than $52, the options might be mispriced.

In this case, the call option seems to be too cheap compared to the put option and the stock. If you spot this, you could buy the call option for $3, sell the put option for $2, and buy the stock for $50. This would cost you $51 in total ($3 for the call, minus $2 from selling the put, plus $50 for the stock). But if you hold onto these until the option expires, you'll either end up with the stock worth $50 or you'll get to sell it for $50, depending on what happens with the options. Either way, you're guaranteed to get at least $50 back, which means you could make a risk-free profit of $52 - $51 = $1. This is an example of how Put-Call Parity can help you find arbitrage opportunities by showing when the prices of options and stocks don't match up like they should.

## How does interest rate affect the Put-Call Parity relationship?

Interest rate plays a big role in the Put-Call Parity relationship because it affects the present value of the strike price. In the Put-Call Parity formula, you add the price of a call option to the present value of the strike price, and this should equal the price of a put option plus the current stock price. The present value of the strike price is what the strike price would be worth today if you account for the time value of money. If the interest rate goes up, the present value of the strike price goes down. This means that for the Put-Call Parity equation to stay balanced, the price of the call option might need to go up or the price of the put option might need to go down.

In real life, when interest rates change, it can mess up the balance in the Put-Call Parity equation. If the interest rate goes up, and the present value of the strike price goes down, but the prices of the options and the stock don't adjust right away, there might be a chance for arbitrage. Traders can spot this and buy or sell the right options and stocks to make a risk-free profit. This helps bring the prices back into line with what the Put-Call Parity formula says they should be. So, keeping an eye on interest rates is important for understanding and using Put-Call Parity in trading.

## What role does dividend payment play in the Put-Call Parity equation?

Dividend payments can change the Put-Call Parity equation because they affect the stock price. When a company pays a dividend, the stock price usually goes down by the amount of the dividend on the day it's paid. This means that if you're using Put-Call Parity to check if options are priced right, you need to think about any dividends that will be paid before the options expire. If there's a dividend coming up, the present value of that dividend needs to be taken out of the stock price in the equation. So, the Put-Call Parity formula changes to: the price of a call option plus the present value of the strike price equals the price of a put option plus the current stock price minus the present value of the dividend.

If you don't account for dividends, the Put-Call Parity equation won't balance out like it should. This can make it look like there's a chance to make a risk-free profit when there isn't one. Traders need to be careful and adjust the equation for any dividends to make sure they're not fooled by a mispricing that's really just because of a dividend payment. By doing this, they can use Put-Call Parity more accurately to find real arbitrage opportunities and keep the options market fair.

## How can advanced traders use Put-Call Parity for synthetic positions?

Advanced traders can use Put-Call Parity to create synthetic positions, which are ways to mimic the payoff of a stock or an option by using other options. For example, if you want to own a stock but don't have the money right now, you can create a synthetic long stock position by buying a call option and selling a put option with the same strike price and expiration date. According to Put-Call Parity, this combination should act just like owning the stock itself. This can be useful if you think the stock price will go up, but you don't want to put down all the money to buy the stock right away.

Traders can also use Put-Call Parity to create synthetic short stock positions. If you think a stock's price will go down, you can sell a call option and buy a put option with the same strike price and expiration date. This combination should give you the same payoff as if you had sold the stock short. By using synthetic positions, traders can take advantage of their predictions about the stock price without having to buy or sell the actual stock. This can help them manage risk and use their money more efficiently, but they need to understand Put-Call Parity well to make sure they get the balance right.

## What is Put-Call Parity and How Do You Understand the Principle?

Put-call parity is a fundamental concept in options pricing, originating from the work of economists who sought to understand the intrinsic relationship between call and put options. This principle is pivotal for options trading, particularly involving European-style options, which can only be exercised at expiration.

In essence, put-call parity defines a specific equality relation between the prices of European call (C) and put (P) options that have identical strike prices (X) and expiration dates. This relationship can be mathematically expressed as:

$$
C + PV(X) = P + S
$$

where:
- $C$ is the price of the call option.
- $PV(X)$ is the present value of the strike price, calculated using the risk-free interest rate.
- $P$ is the price of the put option.
- $S$ is the current price of the underlying asset.

This equation implies that the combination of a long call option and the present value of the strike price is equivalent to the combination of a long put option and the current value of the underlying asset. This relationship must hold to prevent [arbitrage](/wiki/arbitrage) opportunities—profit opportunities that arise from price imbalances across markets without any intrinsic risk.

Put-call parity is contingent upon several conditions. Predominantly, it assumes the absence of transaction costs, taxes, and other market frictions, which could otherwise skew this equilibrium. Additionally, it is applicable under the premise of European options, which do not permit early exercise, unlike American options. These constraints help maintain a balanced and efficient market, as any discrepancy in put-call parity would prompt traders to exploit the mispricing, thereby restoring equilibrium quickly.

Understanding the principle of put-call parity equips traders with a powerful tool to gauge the theoretical fairness of option pricing and to detect any potential arbitrage opportunities, ensuring that the market operates effectively and in harmony with theoretical expectations.

## What is Put-Call Parity in Action: Examples and Applications?

Put-call parity represents a fundamental principle in options pricing that establishes a relationship between the price of call options, put options, and the underlying asset. This principle can be illustrated effectively with a practical example.

### Practical Example of Put-Call Parity

Consider a European call option and a European put option on the same underlying stock, both with a strike price of $50 and an expiration date in three months. Suppose the current stock price is $52, the risk-free [interest rate](/wiki/interest-rate-trading-strategies) is 5% per annum, and no dividends are expected during this period.

The put-call parity equation is expressed as follows:

$$
C + PV(X) = P + S
$$

Where:
- $C$ is the price of the call option.
- $PV(X)$ is the present value of the strike price $X$.
- $P$ is the price of the put option.
- $S$ is the current stock price.

First, calculate $PV(X)$, the present value of the strike price:

$$
PV(X) = X \times e^{-rT}
$$

Where:
- $X = 50$
- $r = 0.05$
- $T = \frac{3}{12}$ (three months expressed in years)

$$
PV(X) = 50 \times e^{-0.05 \times 0.25} \approx 50 \times e^{-0.0125} \approx 50 \times 0.9876 \approx 49.38
$$

Suppose the call option is priced at $3.60. Using the put-call parity formula:

$$
3.60 + 49.38 = P + 52
$$

$$
P = 3.60 + 49.38 - 52
$$

$$
P = 0.98
$$

### Common Scenarios for Put-Call Parity

Put-call parity can be particularly useful in identifying pricing errors in the options market. If the relationship depicted by the parity condition does not hold, it suggests the presence of mispriced options, which can be exploited for arbitrage.

Arbitrageurs can construct a riskless position to take advantage of the price discrepancies. For example, if the left side of the equation (call price plus present value of the strike) is greater than the right side (put price plus stock price), an arbitrageur might sell the call, buy the put and the stock, and lend out the present value of the strike price to profit from the mispricing.

### Market Equilibrium and Arbitrage Opportunities

Put-call parity plays a significant role in maintaining equilibrium in options pricing. Market makers and arbitrageurs contribute to market efficiency by correcting price discrepancies. Through strategies enabled by put-call parity, traders can engage in arbitrage if the equilibrium is disrupted, thus restoring the balance.

These opportunities, while often razor-thin, especially in liquid and efficient markets, motivate the use of [algorithmic trading](/wiki/algorithmic-trading) systems to detect and exploit these discrepancies quickly. The effective use of put-call parity in trading strategies underscores its significance in financial derivatives and options trading, promoting a deeper understanding of market dynamics and enhancing trading efficiency.

## References & Further Reading

[1]: ["Options, Futures, and Other Derivatives"](https://www.amazon.com/Options-Futures-Other-Derivatives-11th/dp/B0B9JS99C2) by John C. Hull

[2]: Black, F. and Scholes, M. (1973). ["The Pricing of Options and Corporate Liabilities."](https://www.cs.princeton.edu/courses/archive/fall09/cos323/papers/black_scholes73.pdf) Journal of Political Economy, 81(3), 637-654.

[3]: Cox, J. C., & Rubinstein, M. (1985). ["Option Markets."](https://archive.org/details/optionsmarkets00coxj) Prentice Hall.

[4]: Taleb, N. N. (1997). ["Dynamic Hedging: Managing Vanilla and Exotic Options."](https://www.amazon.com/Dynamic-Hedging-Managing-Vanilla-Options/dp/0471152803) Wiley Finance.

[5]: Hasbrouck, J. (2005). ["Trading Costs and Returns for U.S. Equities: Estimating Effective Costs from Daily Data"](https://www.jstor.org/stable/20488006). Journal of Finance, 60(3), 1445-1477.

[6]: Aldridge, I. (2010). ["High-Frequency Trading: A Practical Guide to Algorithmic Strategies and Trading Systems."](https://www.amazon.com/High-Frequency-Trading-Practical-Algorithmic-Strategies/dp/1118343506) Wiley Trading.