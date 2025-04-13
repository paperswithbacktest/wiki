---
title: "Maximum Adverse Excursion and Maximum Favorable Excursion Explained"
description: Explore the essentials of Maximum Adverse Excursion (MAE) in algorithmic trading as a key tool for managing risks and optimizing trading strategies. Learn how MAE quantifies potential losses, informs stop-loss placement, and enhances decision-making by evaluating historical drawdowns, making it crucial for developing robust trading frameworks.
---


![Image](images/1.jpeg)

## Table of Contents

## What is Maximum Adverse Excursion (MAE)?

Maximum Adverse Excursion (MAE) is a measure used in trading and investing to understand how much a trade can go against you before it turns profitable. It helps traders see the worst-case scenario for a trade, showing the largest loss a trade experienced from its entry point until it either becomes profitable or is closed.

MAE is important because it helps traders set realistic expectations and manage risk. By knowing the potential maximum loss, traders can decide if they are comfortable with the trade or if they need to adjust their strategy. This measure is often used alongside other metrics like Maximum Favorable Excursion (MFE) to get a complete picture of a trade's potential risks and rewards.

## What is Maximum Favorable Excursion (MFE)?

Maximum Favorable Excursion (MFE) is a measure that shows how much a trade could have made at its best point. It tells you the highest profit a trade reached from the time you entered the trade until you closed it or it turned into a loss.

MFE is useful because it helps traders see what could have been the best outcome for a trade. By knowing the MFE, traders can learn if they are exiting trades too early or if they should hold on longer to get more profit. It's a good tool to use with Maximum Adverse Excursion (MAE) to understand both the best and worst parts of a trade.

## How are MAE and MFE calculated?

To calculate Maximum Adverse Excursion (MAE), you look at the biggest loss a trade had from when you entered it until you closed it or it became profitable. Let's say you buy a stock at $100. If the stock drops to $90 at some point before going back up, the MAE is $10 because that's the largest drop from your entry price of $100.

Maximum Favorable Excursion (MFE) is calculated by finding the highest profit a trade reached from the entry point until you closed it or it turned into a loss. Using the same example, if you bought the stock at $100 and it went up to $120 at some point before you sold it, the MFE is $20 because that's the biggest gain from your entry price of $100.

## Why are MAE and MFE important in trading?

MAE and MFE are important in trading because they help traders understand the risks and rewards of their trades. MAE shows the biggest loss a trade could have had before it turned around or was closed. This helps traders see how much money they might lose if things go wrong. By knowing this, traders can decide if a trade is too risky or if they need to change their plan to protect their money.

MFE, on the other hand, shows the best profit a trade could have made. It helps traders see if they are selling their trades too soon or if they should wait longer to make more money. By looking at both MAE and MFE, traders can get a full picture of what could happen with their trades. This helps them make smarter choices and improve their trading strategies over time.

## Can you provide an example of how MAE and MFE are used in a trade?

Let's say you buy a stock for $50. After you buy it, the price drops to $40 before going back up. The Maximum Adverse Excursion (MAE) in this case is $10 because that's the biggest loss you could have had from your entry price of $50. Knowing this, you might decide to set a stop-loss at $45 to limit your risk, because you now know the stock could drop by $10.

Later, the stock price goes up to $60 before you decide to sell it at $55. The Maximum Favorable Excursion (MFE) here is $10 because that's the highest profit you could have made from your entry price of $50. Seeing this, you might think about waiting longer next time to get closer to the $60 price, instead of selling at $55. By looking at both MAE and MFE, you can make better choices about when to buy, sell, and how much risk to take.

## How do MAE and MFE help in setting stop-loss and take-profit levels?

MAE and MFE help traders set stop-loss levels by showing the biggest loss a trade might have. If you know the MAE, you can put your stop-loss just above that level to protect your money. For example, if a stock you bought at $100 drops to $90 before going up again, the MAE is $10. You might set your stop-loss at $91 to avoid losing more than that.

MFE helps with setting take-profit levels by showing the highest profit a trade could have made. If you see that a trade's MFE was $20, you might set your take-profit at a level close to that to make sure you get most of the profit. For example, if a stock you bought at $100 goes up to $120 before dropping back down, the MFE is $20. You might decide to sell when the stock reaches $118 to capture most of that gain.

## What is the relationship between MAE, MFE, and trade duration?

MAE and MFE can tell us something about how long a trade might last. If a trade has a big MAE early on, it might mean the trade will be short because the price moved a lot against you quickly. You might decide to get out of the trade faster to cut your losses. On the other hand, if a trade has a small MAE, you might feel more comfortable holding it for a longer time because the risk seems lower.

MFE also has a part in deciding how long to keep a trade open. If a trade's MFE is high but happens quickly after you enter, you might think about selling soon to take the profit. But if the MFE keeps growing over time, you might choose to hold the trade longer to get more profit. By looking at both MAE and MFE, you can get a better idea of how long to stay in a trade and when it might be time to get out.

## How can historical MAE and MFE data improve trading strategies?

Looking at past MAE and MFE data can help traders make better choices in the future. By studying how much a trade went against them before turning around, traders can set better stop-loss levels. For example, if a certain stock often has a big MAE but then goes up, a trader might set a wider stop-loss to give the trade more room to move. This way, they can avoid getting out of a trade too soon and missing out on potential profits.

Also, knowing the MFE from past trades can help traders decide when to sell. If a stock usually reaches a high MFE after a certain time, traders might wait a bit longer before selling to get the best profit. By using historical MAE and MFE data, traders can fine-tune their strategies to handle risks better and catch more gains.

## What are the limitations of using MAE and MFE in trading analysis?

Using MAE and MFE can help traders, but they have some limits. One big problem is that past data doesn't always tell us what will happen next. Just because a trade had a small MAE or a big MFE before doesn't mean it will happen again. This means traders can't rely only on these numbers to make choices. They need to look at other things like market news and trends too.

Another issue is that MAE and MFE can make traders focus too much on one trade instead of their whole plan. Traders might get too worried about the worst loss or the best gain of one trade and forget about their overall goals. It's important to use MAE and MFE with other tools to get a full picture of trading risks and rewards.

## How do different market conditions affect MAE and MFE?

Different market conditions can change how MAE and MFE work. In a fast-moving or volatile market, where prices go up and down a lot, the MAE might be bigger because the price can drop a lot before it goes back up. On the other hand, the MFE might also be bigger because the price can jump up quickly too. Traders need to be careful in these markets and might need to set wider stop-losses to give their trades more room to move.

In a slow or steady market, where prices don't change much, the MAE might be smaller because the price doesn't drop as much. The MFE might also be smaller because the price doesn't go up as quickly. In these conditions, traders might set tighter stop-losses and take-profit levels because the trade is less likely to move a lot in either direction. Understanding the market's mood can help traders use MAE and MFE better.

## Can MAE and MFE be used to assess the performance of a trading system?

Yes, MAE and MFE can help traders see how well their trading system is doing. By looking at the biggest losses (MAE) and the biggest gains (MFE) of past trades, traders can figure out if their system is good at handling risks and making money. If a trading system often has a small MAE, it means the system is good at keeping losses low. If it has a big MFE, it means the system can catch big profits.

But, MAE and MFE are just part of the story. They don't tell everything about how a trading system works. Traders also need to look at other things like how often they win, how much they make overall, and how the market is doing. Using MAE and MFE with other tools gives a better idea of how well a trading system is really doing.

## What advanced techniques can be applied to analyze MAE and MFE for optimizing trading decisions?

One advanced way to use MAE and MFE is by looking at them over time. Traders can study how MAE and MFE change from one trade to the next. This can show if a trading system is getting better at handling losses or making bigger profits. By seeing these patterns, traders can tweak their strategies to make them work better. For example, if MAE is getting smaller over time, it might be a sign to keep using the same stop-loss levels or even make them a bit tighter.

Another technique is to use MAE and MFE with other data, like how often trades win or lose, and how much money is made overall. This can help traders see the whole picture of their trading. For example, a trade might have a big MFE, but if it only happens once in a while, it might not be worth waiting for. By mixing MAE and MFE with other numbers, traders can make smarter choices about when to buy or sell and how much risk to take.

## What is Maximum Adverse Excursion (MAE) and how can it be understood?

Maximum Adverse Excursion (MAE) is an essential concept in evaluating trading strategies, particularly for assessing risk and determining optimal stop-loss levels. It describes the maximum loss a trading position can endure from the entry point until it either turns profitable or is closed. Understanding this metric is vital for traders who aim to manage risks effectively and optimize their trading strategies.

To quantify MAE, consider the price movements of an asset after a trading position is entered. MAE measures the extent to which an asset's price moves against the trader's position. For long positions, this involves tracking the lowest price point reached during the trade relative to the entry price. Conversely, for short positions, the MAE is the highest price point above the entry. Mathematically, for a long position, MAE can be expressed as:

$$
\text{MAE} = \min(P_t - P_e)
$$

Where $P_t$ is the price at time $t$ during the trade, and $P_e$ is the entry price. For short positions, the formula is:

$$
\text{MAE} = \max(P_t - P_e)
$$

MAE is more than a theoretical measure; it is a practical tool essential for traders who wish to anticipate and understand past and potential drawdowns. By analyzing MAE, traders gain insights into the worst-case scenarios their strategies might encounter, facilitating informed decisions about setting stop-loss levels. Moreover, MAE aids in establishing an empirical basis for evaluating the reliability of trading strategies under various market conditions, ultimately contributing to more robust and resistant trading frameworks.

## How do you calculate the Maximum Adverse Excursion?

To calculate Maximum Adverse Excursion (MAE) for a trade, it is essential to identify the maximum loss experienced from the entry point before the position either turns profitable or is closed. This calculation is crucial for both long and short positions as it provides insights into the adverse price movements that the position can encounter, thereby informing effective risk management strategies.

For long positions, MAE is computed by determining the difference between the entry price and the lowest price point achieved during the trade's duration. This measurement can be expressed mathematically as:

$$
\text{MAE}_{\text{long}} = \text{Entry Price} - \text{Lowest Price}
$$

In this formula, a positive MAE value indicates the scale of adverse movement against the initial long position before the market conditions improve or the trade is closed.

Conversely, for short positions, MAE involves calculating the difference between the highest price point reached during the trade and the entry price. The formula for calculating MAE in a short position is:

$$
\text{MAE}_{\text{short}} = \text{Highest Price} - \text{Entry Price}
$$

Here, a positive MAE value again signifies the extent to which the market moved unfavorably against the initial short position before any recovery becomes evident or the trade concludes.

To automate the calculation of MAE for multiple trades, the following Python code snippet serves as an illustrative guide. It calculates MAE for both long and short positions from a dataset containing entry prices and high/low prices during trades:

```python
def calculate_mae(entry_price, high_price, low_price, position_type):
    if position_type == 'long':
        mae = entry_price - low_price
    elif position_type == 'short':
        mae = high_price - entry_price
    else:
        raise ValueError("position_type must be either 'long' or 'short'")
    return mae

# Example usage:
trades = [
    {'entry_price': 100, 'high_price': 110, 'low_price': 90, 'type': 'long'},
    {'entry_price': 200, 'high_price': 220, 'low_price': 180, 'type': 'short'}
]

for trade in trades:
    mae = calculate_mae(trade['entry_price'], trade['high_price'], trade['low_price'], trade['type'])
    print(f"Trade MAE for {trade['type']} position: {mae}")
```

Such automation aids traders in comprehensively analyzing an extensive dataset to better understand the drawdown patterns of their trading strategies, thereby optimizing risk management bars and potentially enhancing trade profitability.

## References & Further Reading

[1]: Sweeney, J. (1992). ["Maximum Adverse Excursion: An Expanded Measurement of Risk."](https://analyzingalpha.com/maximum-adverse-excursion) Technical Analysis of Stocks & Commodities Magazine.

[2]: ["Advances in Financial Machine Learning"](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089) by Marcos Lopez de Prado

[3]: Aronson, D. (2007). ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals."](https://www.amazon.com/Evidence-Based-Technical-Analysis-Scientific-Statistical/dp/0470008741) Wiley.

[4]: Chan, E. (2009). ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business."](https://github.com/ftvision/quant_trading_echan_book) Wiley.

[5]: Jansen, S. (2020). ["Machine Learning for Algorithmic Trading."](https://github.com/stefan-jansen/machine-learning-for-trading) Packt Publishing.