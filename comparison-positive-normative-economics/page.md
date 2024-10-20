---
title: "Comparison of Positive and Normative Economics (Algo Trading)"
description: "Explore the distinction between positive and normative economics in the realm of algorithmic trading. Positive economics focuses on objective data analysis to describe economic events, using empirical evidence without subjective judgments. Normative economics considers value-laden perspectives to address how economies should function based on societal values. This article delves into how these branches intersect within economic policy and trading technologies, offering insights on their roles in shaping economic analysis and decision-making. Discover how understanding both perspectives enhances the development of trading models and informs policy-making strategies."
---

Economics is a discipline fundamental to the understanding of financial systems and policy-making, divided into two main branches: positive and normative economics. Positive economics is concerned with objective analysis, focusing on factual data and verifiable outcomes. It seeks to describe and predict economic events, relying on empirical evidence without incorporating subjective judgments. For instance, positive economics might analyze unemployment rates to determine trends based on statistical data, using econometric models.

In contrast, normative economics involves value-laden perspectives and ethical considerations, addressing how economies should function based on societal values and goals. It formulates opinions or prescriptions about economic policy, often reflecting ethical stances. An example of normative economics would be advocating for an increase in the minimum wage to achieve a living wage standard, which embodies societal priorities.

![Image](images/1.webp)

This article will explore these concepts, highlighting their significance in economic analysis and their intersection with algorithmic trading. By understanding these branches, the fusion of objective data analysis and value judgments becomes apparent in shaping economic policies and trading technologies.

## Table of Contents

## Positive Economics: Understanding the 'What Is'

Positive economics is an essential branch of economic thought that emphasizes the analysis of observable and verifiable data to describe and understand economic phenomena. This approach distinguishes itself from normative economics by focusing solely on factual statements and hypotheses that can be tested and validated through empirical evidence.

One of the primary objectives of positive economics is to construct models that capture the dynamics of economic variables and relationships. These models often employ mathematical formulations and statistical methods to interpret data patterns and assess causality. For instance, economists might use regression analysis to explore the relationship between unemployment rates and inflation, adhering to the established Phillips Curve theory. The results obtained from such analyses can guide the development of predictive models that forecast economic outcomes under various scenarios.

In a practical context, positive economics plays a critical role in evaluating the effects of government policies and external shocks on the economy. By leveraging historical data and statistical tools, economists can analyze the impact of a new tax policy on consumer spending behavior or assess the influence of interest rate changes on investment activities. Through these analyses, positive economics provides insights into the likely consequences of policy interventions, helping policymakers make informed decisions based on anticipated outcomes.

The foundation of positive economics rests on the scientific method, which involves the formulation of hypotheses, collection of data, and verification of theories through objective testing. This rigorous approach ensures that economic analyses remain grounded in reality, serving as a reliable basis for economic reasoning and policy assessment. By focusing on "what is," positive economics contributes to a deeper understanding of economic processes and provides valuable guidance for navigating complex economic environments.

In the context of practical applications, such as [algorithmic trading](/wiki/algorithmic-trading), positive economics underpins the development of quantitative models that forecast market trends and inform trading strategies. These models analyze historical price movements, trading volumes, and other relevant variables to generate actionable insights that traders and investors can leverage to optimize their decisions and enhance market efficiency.

## Normative Economics: Exploring the 'What Ought to Be'

Normative economics plays a key role in shaping economic policy by incorporating value judgments and ethical considerations into discussions. Unlike positive economics, which relies on objective data and empirical analysis, normative economics addresses questions of what should be, often guided by societal values and goals. For instance, statements like "the government should increase the minimum wage to ensure a living wage for all citizens" embody normative economic thinking. Such assertions are not based solely on objective data but reflect broader ethical considerations and societal aspirations.

Normative economics is integral to policy-making as it influences decisions that aim to improve societal welfare. Policymakers often confront decisions where multiple outcomes are possible, each with its own implications for different groups within society. Here, normative economics assists in evaluating these outcomes based on societal value systems. For example, debates over wealth distribution, healthcare access, and environmental regulations often involve normative analysis to weigh the benefits and trade-offs of various policies.

The integration of normative perspectives is crucial because purely data-driven approaches may overlook the nuances of equity and justice that are central to public policy. Ethical considerations often drive discussions in areas such as public health, education, and social welfare, where the interests of different stakeholders must be balanced. Thus, normative economics not only informs the "what ought to be" in a society but also guides the ethical framework within which economic choices are made.

By incorporating ethical judgments alongside empirical data, normative economics ensures that economic policies are aligned with the values and principles that a society holds dear. This alignment is essential for formulating policies that are not only efficient but also equitable and just, reflecting the collective conscience and priorities of the community.

## The Role of Economic Analysis in Policy Making

Economic analysis is pivotal in the formation of sound policy-making, as it leverages both positive and normative economics to propose well-rounded and effective policy recommendations. Positive economics provides the empirical foundation necessary for policymakers to understand the current state of economic affairs. By focusing on observable and verifiable data, such as inflation rates, employment [statistics](/wiki/bayesian-statistics), and GDP growth, positive economics allows policymakers to predict the potential outcomes of various policy options. This empirical approach is essential for identifying causal relationships and anticipating the consequences of policy actions.

Conversely, normative economics adds a dimension of value-based judgment and ethical considerations to the policy-making process. It addresses what economic policies should be implemented based on societal values, such as equity, justice, and welfare. For instance, deciding whether to increase the minimum wage involves normative economics, as it requires a judgment about what constitutes a "fair" wage that aligns with social goals.

The integration of both positive and normative perspectives is crucial for devising policies that are not only effective but also equitable and socially acceptable. Policymakers utilize data-driven insights from positive economics to assess the implications of intended policies. They then incorporate normative economics to ensure that these policies align with broader societal goals and ethical standards.

A balanced approach to economic analysis, which harmonizes empirical data with ethical judgments, can lead to more effective and fair economic policies. This symbiosis allows for a comprehensive evaluation of policy impacts, ensuring that economic decisions bolster both efficiency and societal welfare. As a result, policymakers can craft strategies that are economically sound and resonate with public values, thereby enhancing the overall efficacy and fairness of economic policy-making.

## Algorithmic Trading: An Intersection of Economics and Technology

Algorithmic trading employs sophisticated computer algorithms to execute trades automatically, based on a set of pre-established criteria. This method capitalizes on the ability of these algorithms to process vast amounts of data at incredible speeds, far beyond the capabilities of human traders. At its core, algorithmic trading leverages principles of positive economics, using empirical data analysis to forecast market trends and automate the decision-making process.

The methodology behind algorithmic trading can be understood through the lens of economics by examining the role of statistical and econometric models. Typically, these models are designed to recognize patterns within historical price data, [volume](/wiki/volume-trading-strategy), and even news sentiment. For instance, a simple algorithm might be based on a moving average crossover strategy, where a trading signal is generated when a short-term moving average crosses a long-term moving average.

Here is a basic example in Python using pandas and numpy libraries to generate moving average signals:

```python
import pandas as pd
import numpy as np

# Sample data loading (assume 'data' is a DataFrame with a 'Close' column)
data = pd.read_csv('historical_stock_data.csv')

# Calculate short-term and long-term moving averages
short_window = 40
long_window = 100

data['Short_MA'] = data['Close'].rolling(window=short_window, min_periods=1).mean()
data['Long_MA'] = data['Close'].rolling(window=long_window, min_periods=1).mean()

# Generate signals
data['Signal'] = np.where(data['Short_MA'] > data['Long_MA'], 1, 0)
data['Position'] = data['Signal'].diff()
```

In this example, the algorithm tracks closing prices to calculate both short-term and long-term moving averages. A 'buy' signal is triggered (indicated by a +1 in the 'Position' column) when the short-term average exceeds the long-term average, and vice versa for a 'sell' signal.

The integration of algorithmic trading has significantly transformed financial markets by enhancing efficiency and [liquidity](/wiki/liquidity-risk-premium). It allows market participants to execute orders at optimal times and prices, reducing transaction costs and mitigating human biases and errors. Economic theories, particularly those explaining market efficiency and asset pricing, find practical application here, as traders use statistical [arbitrage](/wiki/arbitrage) and other strategies to exploit market inefficiencies.

Moreover, algorithmic trading systems continuously evolve by incorporating [machine learning](/wiki/machine-learning) and [artificial intelligence](/wiki/ai-artificial-intelligence), further improving their predictive accuracy and adaptability. These advancements underscore the importance of a strong foundation in positive economics, as the reliability of data-driven insights directly influences trading success.

The impact of algorithmic trading on financial markets is profound, both in terms of volume and velocity of transactions. It ensures that economic principles are not just theoretical constructs but active components of a continually developing financial ecosystem. This synthesis of technology and economics exemplifies how theoretical knowledge can translate into tangible outcomes in real-world scenarios.

## Conclusion: The Symbiosis of Economics, Policy, and Algorithmic Trading

The intersection of positive and normative economics offers a comprehensive framework for understanding economic phenomena and their implications for both policy and trading. Positive economics, with its emphasis on data-driven insights, provides a factual basis on which economic models and predictions can be built. Normative economics complements this by incorporating societal values and ethical considerations, ensuring that economic policies align with broader human goals.

As financial technologies continue to evolve, economic analysis plays an increasingly critical role in guiding both efficient and ethical market operations. Algorithmic trading exemplifies this evolution by utilizing complex algorithms to make decisions based on empirical data—an application grounded in positive economics. This automation not only enhances trading speed and efficiency but also underscores the necessity of robust data analysis.

However, while empirical data is crucial, it is the integration of normative perspectives that often determines the ultimate success and societal acceptance of these technologies. Policymakers must balance these two approaches—leveraging empirical insights to assess potential economic outcomes while using normative judgments to ensure that these outcomes align with ethical standards and societal values.

A balanced approach that effectively merges empirical and value-based insights enhances decision-making processes in both economics and finance. By acknowledging the contributions of both positive and normative economics, policymakers, economists, and technologists can foster financial systems that are not only efficient and innovative but also just and equitable. This symbiosis thus becomes essential for navigating the complex economic landscapes of the future, ensuring that advancements in financial technology translate to benefits that are widely shared across society.

## References & Further Reading

[1]: Friedman, M. (1953). ["Essays in Positive Economics"](https://en.wikipedia.org/wiki/Essays_in_Positive_Economics). University of Chicago Press.

[2]: Hausman, D. M. (2008). ["The Philosophy of Economics: An Anthology"](https://www.cambridge.org/core/books/philosophy-of-economics/36F55C3A2AED6BD3BCDCD9CE8A9FC1FC). Cambridge University Press.

[3]: Beggs, J. (2017). ["Positive vs. Normative Economics."](https://www.thoughtco.com/positive-versus-normative-analysis-1147005) Investopedia.

[4]: Lopez de Prado, M. (2018). ["Advances in Financial Machine Learning"](https://www.amazon.com/Advances-Financial-Machine-Learning-Marcos/dp/1119482089). Wiley.

[5]: Chan, E. P. (2009). ["Quantitative Trading: How to Build Your Own Algorithmic Trading Business"](https://github.com/ftvision/quant_trading_echan_book). Wiley.

[6]: Jansen, S. (2020). ["Machine Learning for Algorithmic Trading"](https://github.com/stefan-jansen/machine-learning-for-trading). Packt Publishing.

[7]: Aronson, D. (2007). ["Evidence-Based Technical Analysis: Applying the Scientific Method and Statistical Inference to Trading Signals"](https://www.amazon.com/Evidence-Based-Technical-Analysis-Scientific-Statistical/dp/0470008741). Wiley.