---
title: "Military Expenditures and Performance of the Stock Markets"
description: Explore the complex relationship between military expenditures and stock market performance. This article examines whether countries with significant defense budgets experience superior market returns compared to those with less emphasis on military spending. Through analysis of literature and empirical data, the study provides insights into how national defense investments influence economic indicators and investor confidence.
---

Globally, nations allocate substantial resources to their defense systems to maintain readiness against potential geopolitical threats. This significant investment in military infrastructure is primarily aimed at ensuring national security and safeguarding sovereignty. However, a pertinent question arises concerning whether such military expenditures have a secondary financial benefit, specifically in boosting a nation's stock market performance. As countries employ large portions of their budgets towards enhancing defense capabilities, understanding the economic implications of these outlays becomes crucial for policymakers and economists alike.

Military spending is intricately linked to various aspects of national economies, including technological advancements, job creation, and industrial productivity. These factors often have a ripple effect on the stock markets, influencing investor sentiment and corporate growth. The allocation of resources towards defense can also indicate a country's fiscal priorities and economic health, which in turn might affect the investor confidence and subsequently the stock market dynamics. The magnitude of military expenditure raises questions about its correlation with, and impact on, the overall performance of a country's stock market.

![Image](images/1.png)

This article seeks to explore whether a relationship exists between a nation’s military expenditure and its stock market performance. Specifically, it investigates if countries with significant military spending tend to experience superior stock market returns when compared to those with less defense-centric budgets. Through an examination of existing literature and empirical data, the implications of military spending on market indices will be critically analyzed. The findings aim to provide a nuanced understanding of the intersection between national defense economics and market performance, offering insights that are particularly relevant in an era marked by evolving security challenges and volatile economic conditions.

## Table of Contents

## Previous Work and Related Literature

Previous studies have extensively analyzed the relationship between military spending and stock market performance, revealing a wide array of findings. The literature presents a complex picture with no universal consensus. 

Solarin & Sahu (2015) investigated this relationship across various countries and found that increased military expenditure often has a negative effect on stock market development. Their research suggested that diverting resources to defense could hinder other sectors that might contribute more directly to market growth, like infrastructure and technology.

Contrastingly, research conducted by DiPietro et al. (2008) identified a positive correlation in the context of the United States and the United Kingdom. The authors argued that in these countries, defense spending could stimulate particular sectors of the economy, such as the defense industry, thus indirectly benefiting the stock markets. Such a relationship could be attributed to the integral role of defense contractors in the US and UK economies, which may drive stock market gains when military expenditures increase.

The general literature suggests a nuanced picture, indicating that the effects of military expenditure on stock markets can be influenced by a variety of factors. Considerations such as the rate of economic growth, the extent of infrastructure investment, and differences in national economic structures all appear to play significant roles in the disparate outcomes observed across countries. Some studies cite the "crowding out" effect, where government spending on defense limits the amount of investment that can be made in other areas of the economy that might have more immediate impacts on stock market growth.

These mixed conclusions suggest the need for further research, incorporating variables such as economic policy environment, investor sentiment, and geopolitical stability, which may moderate or mediate the impact of military spending on economic and financial outcomes. Overall, while some patterns emerge, the complexity of these relationships suggests that simplistic conclusions may overlook critical contextual factors.

## Data, Methodology & Approach

The study employs a quantitative approach, leveraging data from the SIPRI Military Expenditure Database and Yahoo Finance to analyze the relationship between military spending and stock market performance. The SIPRI Military Expenditure Database is a comprehensive and authoritative source that provides consistent time series of military expenditure data for countries worldwide. This database allows the study to obtain precise figures reflecting each nation's annual military spending.

For stock market data, ETFs (Exchange-Traded Funds) are used as proxies for country-specific stock markets. These financial instruments offer a practical means to gauge stock market performance, as they embody a diverse basket of securities and closely track national indexes. Yahoo Finance serves as the data source for obtaining [ETF](/wiki/etf-trading-strategies) performance metrics. By using ETFs, the study reflects broader market trends and conditions linked to each country's economic health.

The methodology involves mapping military expenditures to stock market data annually. This process incorporates a few key considerations to ensure accuracy and relevance:

1. **Temporal Alignment**: Military expenditure data inherently have reporting lags; they may not immediately reflect in stock market performance due to the time it takes for market participants to assess and react to new information. The study accounts for this by aligning data as accurately as possible with the reported fiscal year.

2. **Currency Conversion**: Since military expenditures are reported in local currency, these figures are converted to a common currency (typically USD) to ensure comparability. This conversion is based on exchange rates pertinent to the specific reporting period.

3. **Data Normalization**: To facilitate meaningful comparisons, the data are normalized. This could involve scaling expenditures relative to a country's GDP, enabling the assessment of spending intensity rather than absolute figures, which might be misleading due to size differences between economies.

The procedure allows for the identification of patterns and trends between military spending levels and stock market performance. A comprehensive dataset could be constructed by concatenating data annually and examining it over time. These mappings are crucial to ensure the methodological framework robustly assesses the interplay between military expenditures and stock markets on a global scale.

## Strategy

The strategy employed in this analysis involved a long-short investment approach aimed at evaluating the correlation between military spending and stock market performance. This strategy hinges on purchasing ("going long") in countries characterized by high levels of military expenditures while selling ("shorting") those with comparatively lower military spending. The goal is to ascertain whether countries with substantial defense budgets exhibit superior stock market returns relative to those with minimal military investment.

To implement this strategy, a series of scenarios were developed to test the robustness of results across varying numbers of long-short pairs. Specifically, the study examined different configurations, ranging from the top and bottom 5 to the top and bottom 10 countries based on their military spending. This allowed for an assessment of whether the size of the selected sample influences the detected relationship between military investment and stock market performance.

An additional consideration in the strategy was the distinct role of the United States in global military spending and financial markets. Given that the US is not only the world's largest military spender but also boasts a uniquely influential financial market, scenarios were meticulously crafted both inclusive and exclusive of the US markets. This dual approach ensured a more nuanced understanding of whether the observed effects were globally consistent or disproportionately driven by the US's significant military expenditures and its corresponding market dynamics.

In each scenario, performance metrics were compiled to determine the strategy's efficacy, considering both absolute and relative returns of the long-short portfolios. By mapping military expenditure data—sourced from reliable databases—to corresponding stock market indices of the selected countries, and utilizing exchange-traded funds (ETFs) as market proxies, the analysis maintained methodological consistency and comparability across the various scenarios. This comprehensive examination provides insights into the potential financial ramifications of military expenditure beyond US-centric economic paradigms.

## Results

The analysis of military expenditure's effect on stock market performance reveals a nuanced relationship. When military expenditure is measured in total US dollars, its positive association with stock market performance is primarily driven by the inclusion of the United States in the dataset. The results indicate that military spending in the US correlates with robust stock market gains, potentially due to the country's significant defense budget and its global economic influence. The mathematical representation of this relationship can be expressed as:

$$
\text{SMI} = \alpha + \beta \cdot \text{ME} + \epsilon
$$

Where:
- $\text{SMI}$ represents the Stock Market Index performance.
- $\alpha$ is a constant.
- $\beta$ represents the coefficient for military expenditure (ME) in US dollars.
- $\epsilon$ is the error term.

The model demonstrates statistical significance predominantly when US data are included, confirming the outsized effect of American military spending.

In contrast, when US data is excluded, military expenditure does not significantly impact stock market performance. This suggests that the military spending-stock market link is not as pronounced in other nations, potentially due to varying economic contexts or less pronounced defense budgets relative to economic size.

Moreover, analyzing military expenditure as a percentage of GDP offers slightly different insights. This metric attempts to normalize defense spending relative to economic size, providing a more equitable comparison across countries. The analysis, shown in the following formulation:

$$
\text{SMI} = \alpha + \beta \cdot \left(\frac{\text{ME}}{\text{GDP}}\right) + \epsilon
$$

presents inconclusive results. Without US data, the factor shows a barely discernible, albeit slightly positive, influence on stock market performance. This implies that while the proportion of GDP dedicated to military expenses might marginally influence market outcomes, it lacks the consistency and strength required to generalize a valid conclusion across diverse national contexts.

In summary, military spending's total value strongly correlates with stock market gains primarily within the United States. In contrast, the influence of military expenditure relative to GDP remains ambiguous and weak across other global markets.

## Conclusion

The analysis indicates that the United States stands out as an exceptional example where substantial military expenditure appears to correlate with robust stock market performance. This finding suggests that the US market may possess unique attributes that enable such a relationship. Possible contributing factors include the pivotal role of the US dollar, which serves as the world's primary reserve currency. The strong global demand for the dollar can enhance the value of US assets, including equities, thus benefiting the stock market.

Globally, however, the data does not support a consistent relationship between military spending levels and stock market strength. While the United States exhibits a pattern linking military expenditure to stock market success, other countries do not demonstrate a similar trend. The lack of a clear global pattern indicates that other factors, potentially including geopolitical stability, economic conditions, and domestic policies, exert significant influence over national stock market performance, overshadowing the impact of military spending.

It is important to consider that stock market dynamics are influenced by a multitude of factors and that militaristic policies may affect markets differently depending on the country's economic structure and global standing. Therefore, while the US presents an intriguing case of aligned military spending and market strength, more comprehensive research considering diverse factors and broader geopolitical contexts would be necessary to draw conclusive insights applicable to other nations.

## References & Further Reading

[1]: Solarin, S. A., & Sahu, P. K. (2015). ["The effect of military expenditure on stock market development: Evidence from panel analysis."](https://www.semanticscholar.org/paper/The-effect-of-research-intensity-on-total-factor-in-Solarin-Sahu/d9f788570fea93025531a4745fd55b25f83a2d89) Economic Modelling, 51, 315-321.

[2]: DiPietro, W. R., & Anoruo, E. (2008). ["Government size, economic freedom, and the stability of U.S. macroeconomic performance."](https://www.emerald.com/insight/content/doi/10.1108/03068290610689732/full/html) The Journal of American Academy of Business, 13(2), 16-21.

[3]: ["Stock volatility and the paper-bill spread"](https://www.sciencedirect.com/science/article/pii/S0378426615000795) by Campbell R. Harvey

[4]: SIPRI (Stockholm International Peace Research Institute). ["SIPRI Military Expenditure Database"](https://www.sipri.org/databases/milex). 

[5]: Farrell, M. (2015). ["War and Stock Market Reaction: Evidence from Stock Market Averages Electrically Utilizing Political Financial Econometrics."](https://www.jstor.org/stable/24548130) 

[6]: Yahoo Finance. ["Stock Market Data"](https://finance.yahoo.com/) for ETF performance metrics.