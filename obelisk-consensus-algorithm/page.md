---
title: "Obelisk Consensus Algorithm (Algo Trading)"
description: "Explore the innovative Obelisk consensus algorithm within the Skycoin ecosystem. Discover how it enhances blockchain technology and influences algorithmic trading."
---

In the fast-evolving world of cryptocurrency and blockchain, new technologies continuously emerge, focused on enhancing efficiency, security, and sustainability. Among these innovative solutions is the Obelisk consensus algorithm, a cornerstone of the Skycoin blockchain ecosystem. This article presents an in-depth exploration of the Obelisk consensus algorithm, assessing its influence on blockchain technology and its nascent role in algorithmic trading.

Unlike traditional consensus mechanisms like Proof-of-Work (PoW) and Proof-of-Stake (PoS), which face criticism for issues such as high energy consumption and the potential for centralization, Obelisk introduces a novel approach through its "web of trust" model. This design aims to distribute network influence more equitably, mitigating the drawbacks associated with PoW's energy demands and PoS's propensity for wealth concentration and centralized control. 

![Image](images/1.png)

The Obelisk algorithm represents a shift towards decentralized network management, entrusting a broader range of participants with the task of transaction validation. This adjustment not only fosters a more democratic blockchain environment but also underpins the Skycoin project's overarching vision—a decentralized internet infrastructure. Furthermore, by integrating Obelisk into algorithmic trading, its potential impacts extend to enhancing the efficiency and security vital for high-frequency trading operations.

This article will further elaborate on how the Obelisk consensus algorithm functions, its advantages over other consensus mechanisms, and its applications within the Skycoin ecosystem and algorithmic trading platforms. By addressing inherent limitations in established consensus mechanisms, Obelisk paves the way for more robust and sustainable blockchain solutions.

## Table of Contents

## Understanding the Obelisk Consensus Algorithm

Obelisk is a consensus algorithm devised to address the inefficiencies and centralization issues found in more traditional consensus mechanisms such as Proof-of-Work (PoW) and Proof-of-Stake (PoS). While PoW requires substantial computational power and energy, often leading to environmental concerns, PoS can result in wealth concentration where those with more resources exert greater influence over the network. Obelisk, by contrast, employs a 'web of trust' model, which introduces a decentralized approach to power distribution within the network. This ensures a more balanced and democratic method for transaction validation.

In the Obelisk consensus system, network influence is spread across a broader base of users, mitigating the potential for dominant entities to control the decision-making process. The 'web of trust' approach functions by having nodes form trust relationships with one another, thereby integrating social trust networks into the decision-making process of the blockchain. This approach is designed to simulate a social graph, where the level of trust in the network is related to the number of connections and the strength of those connections each node has.

Within the Obelisk framework, there are two distinct types of nodes: block-generating nodes and consensus nodes, each fulfilling specific roles within the network. Block-generating nodes are tasked with collecting and validating transactions. They then assemble these transactions into blocks which they propose to the network for confirmation.

Consensus nodes, on the other hand, are responsible for the validation and agreement process. After gathering blocks from various block-generating nodes, consensus nodes evaluate these blocks to determine the 'local winner'. A block is deemed a 'global winner' when a majority of consensus nodes agree on its validity, subsequently incorporating it into the blockchain. This mechanism not only enhances the security and efficiency of blockchain operations but also aligns with the objectives of [algorithmic trading](/wiki/algorithmic-trading) systems by ensuring swift and secure processing of transactions.

By circumventing the drawbacks of traditional algorithms and instituting a decentralized web of trust, Obelisk provides a robust foundation for equitable and efficient blockchain network management. This innovative design reflects a forward-thinking approach to overcoming the challenges inherent in maintaining decentralized networks.

## How Obelisk Works

Block-generating nodes in the Obelisk consensus algorithm are responsible for collecting and verifying incoming transactions. Once verified, these transactions are organized and formed into blocks. This process is primarily concerned with the integrity and validity of transactions, ensuring they are properly formatted and adhere to the protocol's rules.

Consensus nodes then take on the critical task of evaluating these blocks. They gather the blocks produced by the block-generating nodes and work to identify a 'local winner'. This is determined by the network's consensus protocol, where nodes leverage a trust-based model to reach an agreement on which block should proceed. In practice, nodes evaluate the trust levels within their network, facilitating a decision-making process that is both decentralized and efficient.

A block becomes a 'global winner' once it achieves consensus across a majority of consensus nodes. Only after this agreement is secured is the block appended to the blockchain. This multi-layered consensus process, involving both local and global consensus phases, adds a robust layer of security. It effectively mitigates the risks associated with double-spending and fraudulent transactions.

The architecture of Obelisk, with its division of labor between block-generating and consensus nodes, ensures that the blockchain can efficiently and securely handle transactions. This distributed method is particularly beneficial for algorithmic trading systems, where speed and reliability are paramount. By reducing bottlenecks and distributing consensus tasks across the network, Obelisk supports sustainable and responsive blockchain operation, which is essential for processing high-frequency trading transactions without compromising on security.

## Applications in the Skycoin Ecosystem

Skycoin utilizes the Obelisk consensus algorithm to power its vision of a decentralized internet service by integrating it into its ecosystem, particularly through the Skywire platform. Skywire represents a major component of the Skycoin network, designed to enable users to operate as their own internet service providers. This is achieved by creating a mesh network that leverages the bandwidth and resources of its participants. By distributing internet services across a decentralized network of nodes, Skywire promotes a more democratized and resilient internet infrastructure.

Participants in the Skywire network are incentivized through a dual-reward system comprising Skycoin and Coin Hours. Skycoin serves as the primary [cryptocurrency](/wiki/cryptocurrency), while Coin Hours represent a time-based reward system that accrues over time as users contribute bandwidth and network resources. This dual-reward framework ensures that users are compensated not only for their initial involvement but also for sustained participation in maintaining network functionality and robustness.

This innovative setup has the potential to revolutionize the delivery and monetization of internet services by shifting the paradigm from centralized ISP control to a distributed, user-centric model. By harnessing the capabilities of the Obelisk consensus algorithm, Skycoin and Skywire enable a self-sustaining network that encourages active user involvement and resource sharing, paving the way for a new era of internet connectivity that is both efficient and equitable.

## Comparison with Traditional Consensus Mechanisms

Proof-of-Work (PoW) and Proof-of-Stake (PoS) have been integral to the development of blockchain networks, each with distinct advantages and disadvantages.

Proof-of-Work, utilized by Bitcoin and other major cryptocurrencies, involves miners competing to solve complex mathematical puzzles. This process requires substantial computational power and energy, leading to environmental concerns over its sustainability. Furthermore, PoW tends to centralize power within large mining pools that can afford extensive hardware investments, potentially threatening the decentralized ideal of blockchain technology.

### Energy Consumption

Mathematically, the energy expenditure in PoW can be modeled as:

$$
E = N \times H \times C
$$

where:
- $E$ is the total energy consumption,
- $N$ is the number of miners,
- $H$ is the hash rate (hashes per second), and
- $C$ is the energy cost per hash.

The exponential increase in energy consumption as $N$ and $H$ grow can lead to unsustainable energy demands.

### Centralization

Additionally, PoW's competitive mining environment favors entities with more resources, as they can maintain higher hash rates and solve puzzles faster, leading to mining centralization.

Conversely, Proof-of-Stake aims to mitigate PoW's energy demands by selecting block validators based on the number of coins they hold and are willing to "stake" as collateral. While it reduces energy consumption, PoS can result in wealth concentration, where those with substantial holdings exert more significant influence over the network, potentially leading to oligarchic structures.

### Wealth Concentration

In PoS, an individual's chance of validating the next block is proportional to their stake:

$$
P(i) = \frac{S(i)}{\sum_j S(j)}
$$

where:
- $P(i)$ is the probability of individual $i$ being chosen as the validator,
- $S(i)$ is the stake of individual $i$, and
- $\sum_j S(j)$ is the total amount of staked coins in the network.

This probability model inherently favors wealthier participants, potentially centralizing control over time.

The Obelisk consensus algorithm presents an innovative solution to these issues by employing a 'web of trust' model. Unlike PoW and PoS, Obelisk distributes influence through a network of trust-based relationships among nodes. This model facilitates a more democratic and balanced distribution of power, minimizing the risks associated with energy consumption and wealth concentration.

By decentralizing influence across its network, the Obelisk consensus algorithm ensures that no single entity gains disproportionate control, promoting a fair and equitable system. This approach aligns more closely with the democratic and decentralized ethos envisioned in the original blockchain concept, fostering an environment conducive to sustainable growth and innovation.

## Relevance to Algorithmic Trading

The Obelisk consensus algorithm offers significant advantages for algorithmic trading platforms, particularly due to its efficiency and security features. Unlike traditional consensus mechanisms, Obelisk ensures swift and secure transaction processing, which is critical for the fast-paced environment of algorithmic trading. The algorithm's structure, characterized by the decentralized assignment of validation roles, contributes to reduced latency in transaction settlements.

Algorithmic trading thrives on the speed and accuracy of transaction execution. The dual-node system within Obelisk—comprising block-generating and consensus nodes—facilitates a streamlined approach to managing the blockchain ledger. This structure ensures that transactions are verified promptly, maintaining the [momentum](/wiki/momentum) necessary for effective algorithmic strategies. Additionally, the consensus model of Obelisk reduces the risk of bottlenecks typically associated with more centralized consensus approaches, thereby optimizing trade execution.

Furthermore, the decentralized control of the Obelisk algorithm diminishes the need for resource-intensive mining operations seen in other systems such as Proof of Work (PoW). This not only lowers operational costs but also promotes sustainable trading practices, aligning with the global push towards eco-friendliness. As excessive energy consumption is a significant issue with PoW, the Obelisk mechanism's reduced reliance on such activities ensures a more environmentally sustainable system, which can be appealing to eco-conscious traders and institutions.

The process can be illustrated with a Python function showcasing a simplified model of transaction validation in a decentralized network. Although the actual implementation would be more complex, such a function might look like this:

```python
def validate_transactions(transactions, consensus_nodes):
    """ Simulate the transaction validation process in a decentralized system """
    valid_transactions = []
    for transaction in transactions:
        # Simulate consensus node agreement
        votes_for = sum(node.validate(transaction) for node in consensus_nodes)
        if votes_for > len(consensus_nodes) / 2:  # Simple majority rule
            valid_transactions.append(transaction)
    return valid_transactions

# Example usage
transactions = [...]  # List of transaction data
consensus_nodes = [...]  # List of consensus node objects with 'validate' method
valid_transactions = validate_transactions(transactions, consensus_nodes)
```

In this simplified model, transactions are considered valid if more than half of the consensus nodes approve them, a process that underpins the security and rapid processing capabilities essential for algorithmic trading.

In conclusion, the Obelisk algorithm provides a robust infrastructure for algorithmic trading by facilitating secure, rapid transactions without the excess energy requirements typical of traditional mining operations. Its design ensures a decentralized and equitable transaction validation process, creating a sustainable and efficient trading ecosystem.

## Conclusion

The Obelisk consensus algorithm represents a significant advancement in blockchain technology by effectively addressing key challenges inherent in traditional consensus mechanisms. Traditional systems such as Proof-of-Work (PoW) and Proof-of-Stake (PoS) have been critiqued for energy inefficiency and potential centralization, issues that Obelisk resolves through its innovative decentralized model. By employing a 'web of trust' and dual-node functionality, Obelisk distributes influence across the network more equitably, ensuring a balanced and secure transaction validation process. This approach not only enhances sustainability but also simplifies user interaction, making the technology more accessible.

As an integral component of the Skycoin project, Obelisk extends its influence beyond mere transaction validation. It underpins a broader vision for decentralized digital finance and autonomous trading systems. Skycoin leverages this algorithm to enable users to act as their internet service providers, thereby laying the groundwork for groundbreaking shifts in how internet services and financial processes are managed and monetized.

The increasing demand for efficient, secure digital platforms highlights the essential role of Obelisk and its associated technologies in the crypto-economic landscape. With its capacity to enable swift, reliable, and environmentally friendly transactions, Obelisk is poised to become a vital part of the infrastructure supporting next-generation digital finance and algorithmic trading systems. Its applications promise to propel innovations that cater to a global digital economy striving for sustainability and inclusivity.

## References & Further Reading

[1]: Zhen, L., Liu, Y., Chen, X., & Liu, X. (2019). ["Proof of Trust: A Blockchain Consensus Protocol Based on Trust Model."](https://scholar.google.com/citations?user=5aesls8AAAAJ) IEEE Access.

[2]: Popov, S. (2016). [“The Tangle."](https://www.semanticscholar.org/paper/The-Tangle-Popov/43586b34b054b48891d478407d4e7435702653e0) IOTA Foundation.

[3]: Narayanan, A., Bonneau, J., Felten, E., Miller, A., & Goldfeder, S. (2016). ["Bitcoin and Cryptocurrency Technologies."](https://press.princeton.edu/books/hardcover/9780691171692/bitcoin-and-cryptocurrency-technologies) Princeton University Press.

[4]: Skycoin Project. ["Skycoin: Whitepaper."](https://github.com/skycoin/whitepapers) 

[5]: Antonopoulos, A. M. (2017). ["Mastering Bitcoin: Unlocking Digital Cryptocurrencies."](https://books.google.com/books/about/Mastering_Bitcoin.html?id=IXmrBQAAQBAJ) O'Reilly Media.