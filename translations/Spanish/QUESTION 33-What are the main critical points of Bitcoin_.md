## What are the main critical points of Bitcoin? ##

Bitcoin is an innovative and decentralized system, not only in the management of nodes but also in terms of development.

Its being open source makes it possible for anyone to work on it and to propose subsequent modifications to the protocol to the community.

Some detractors of the system, who usually support alternative and definetly less decentralized and neutral systems, argue that a sort of programmer lobby has &quot;appropriated&quot; the project and pushed it in the direction they set.

This point of view is born from a misunderstanding: **Bitcoin is a decentralized network but there are limited software implementations that allow its use in accordance with the basic protocol**.

The main of these implementations is Bitcoin Core, created by the same Nakamoto.
 Since the disappearance of Nakamoto, but to tell the truth, even before that, the management of the development of Bitcoin Core has been entrusted to some programmers and a lead maintainer, to date Wladimir J. van der Laan. For a complete overview of how Bitcoin Core development works, please take a look at the article _Who Controls Bitcoin Core?_ by Jameson Lopp.[CITATION Jam1 \l 1040]

Core is not Bitcoin though.

As mentioned, anyone, in compliance with the basic protocol, can develop their own full node software.

The &quot;Bitcoin Core&quot; name, used to define the system, it is a clear attempt to confuse users by trying to convince them of an alleged centralization of the system.

Remember that, even assuming that a centralization in the development of Bitcoin exists, it is the nodes that have the final &quot;right to vote&quot;. At each update, anyone with a node can decide whether they agree with the new implementation and whether to support the changes by installing it.

Bitcoin is a system that is still relatively young and in full development but, with the passage of time and blocks, it becomes more and more solid.

Far from being perfect!

There are still critical issues; some concern the onchain scalability of the system, which will be improved over time, others its exposure to possible attacks, some the block mining protocol and others the decentralization of its development.

In this book we have verified that the economic model underlying Bitcoin discourages attacks on the network (eg a voluntary reorg with the complicity of more than half of the miners) which, even if possible, would constitute a losing bet: a Bitcoin system sensitive to these attacks would see its currency drastically losing value and the attacking miners would risk remaining with a handful of useless digital collectible objects in their hands.

We can therefore deduce that the more the system is strengthened in terms of the computing power employed by the miners (hashrate), the number of miners and the monetary value of the bitcoin asset, the less it is likely that coordinated attacks against it will take effect.

Regarding onchain scalability, that is the possibility of increasing the number of transactions that can be performed on blockchain, different solutions are being studied.

Although second layer solutions such as Lightning Network are considered by most to be the correct way to exponentially increase the number of transactions, it is also true that these will necessarily have to be accompanied by blockchain scaling solutions.

The introduction of SegWit paved the way for Lightning Network and, as a pleasant side effect, &quot;lightened&quot; onchain transactions, but not enough.
 Therefore, important modifications to the basic protocol are being developed that will constitute, in the coming years, the backbone on which future scaling solutions will be implemented:

1. **Schnorr signatures** , proposed by the co-founder of Blockstream Pieter Wuille, which would allow various participants to produce a single aggregated signature with a single public key;
2. **Merkelized Abstract Syntax Trees (MAST)**, proposed by the Bitcoin Core developer Dr.Johnson Lau, which would reduce the size of smart contract on blockchain;
3. **Taproot** , which would combine these two above to improve the privacy of single Bitcoin transactions.

&quot;_Taproot to make all outputs and cooperative spends indistinguishable from each other. Merkle branches to hide the unexecuted branches in scripts. Schnorr signatures enable wallet software to use key aggregation/thresholds within one input.&quot;_
_- Pieter Wuille_

A further technological step will be given by the much reviled increase in the size of the Bitcoin blocks.

Let us remember that the limit to the weight of the single block is an imposed but common sense measure, designed to preserve the decentralization of the system itself.

As we have seen previously, an increase in size without appropriate and obvious technological improvements, including the expansion of hard disk storage capacity and the increase in capacity and available bandwidth (throughput) of user connections, would entail a rapid centralization of system because fewer individuals would be able to maintain active full nodes. The number of nodes would initially be concentrated in the most technologically advanced areas of the world, reducing to those with higher technological barriers. It would then end up with a dangerous &quot;professionalization&quot; of Bitcoin block validation and the system would lose its main purpose.

Therefore **it will be possible to proceed with an increase in the size of the blocks when any threat to decentralization is avoided.**

Let us now analyze the critical issues concerning Bitcoin mining.

Today most of the miners cooperate with each other within pools: the more the difficulty increases and the more it does it in a short time, the greater this tendency to cooperation. As we saw in the mining chapter, the individual miner should be mine along with others because his chances of discovering the solution that allows him to close the block are extremely rare: it is better to solve many small problems at a time and communicate the result to the pool, rather than trying to solve everything alone.

The problem lies in the fact that, in theory, those who have control of the pools could hijack the computing power of the system for personal purposes: support this or that version of the protocol (forks), collaborate with other great actors to rewrite the history of the transactions (voluntary reorgs), and so on.

Stratum V1, the mining protocol used by the vast majority of pools, therefore offers them a relatively powerful position.
 Not only are they responsible for distributing rewards to miners, but they have decision-making power over which transactions to include in the candidate blocks, as well as on which version of the Bitcoin Protocol to use[44].

Solutions are therefore being studied that would drastically reduce the impact this cooperative management has on the decentralization of Bitcoin mining.

<img src="images/minatore.jpg" width="400" alt="miner">

**Betterhash**

Betterhash, a solution developed by Matt Corallo, was designed to reduce the dominant position of pool operators: if implemented it would allow individual miners to build their candidate blocks by themselves, independently deciding which transactions to include, as well as maintaining personal full node, with the consequent possibility to choose which version of the Bitcoin Protocol to support.

Betterhash would therefore provide more efficiency, security and decentralization to mining pools[45].

According to some, the solution proposed by Matt Corallo would not completely eliminate the potential abuse of dominant positions by the pool administrators: these could still force the miners to censor some transactions with the threat of not receiving rewards if they did not.

That being said, a threatened miner could simply change pools.

**Stratum V2**

Braiins, the company behind Slush Pool, recently announced the second version of Stratum, Stratum V2.
 This is a solution inspired by Betterhash, which solves many of the problems of the first version as well as some critical aspects of Matt Corallo&#39;s proposal.

In an interview with Bitcoin Magazine, Braiins co-CEO Pavel Moravec explained that:

&quot;_Stratum V2 would allow pool operators to verify the validity of new block models asynchronously. As soon as a miner sends a candidate block to the pool, he can immediately start hashing. Meanwhile, the pool operator starts checking all the new candidate blocks._

_If a block model is later deemed invalid, the miners&#39;reward can be modified accordingly. So the miners have an incentive to work on adequate blocks and provide all the data in a timely manner. However, they can continue to work on their candidate blocks without any delay.&quot;_

Stratum V2 would also introduce other improvements in security, efficiency and flexibility. After numerous internal tests on Slush Pool, Braiins will submit its solution to the community by publishing a Bitcoin Improvement Proposal (BIP).

Let&#39;s finish by spending a few words on the decentralization of Bitcoin development.

While considering that, as mentioned, the development of Bitcoin is in the hands of the free initiative of programmers around the world, it is also true that, if we observe which implementations of full node software are more used, Bitcoin Core turns out to be the most widespread, present on about 97% of the nodes[46].

Lightning Network&#39;s implementations, which allow us to configure LN nodes and actively interact with the network, are more decentralized in their development and use than those of the Bitcoin base layer.

In just over a year since the development of the Lightning Network mainet we have eight implementations available:

1. LND (go)

2. c-lightning (c)

3. Eclair (scala)

4. Electrum (python)

5. Ptarmigan (c)

6. BLW (scala)

7. Rust-Lightning (rust)

8. Lpd (rust)

I therefore consider it appropriate that work on alternative versions of Bitcoin Core should continue unabated, for the sake of the Bitcoin base layer itself: more versions available reduce the likelihood of critical bugs occurring and that DDoS-type attacks on Bitcoin Core may endanger network decentralization.
