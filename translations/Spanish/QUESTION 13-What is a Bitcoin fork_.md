## What is a Bitcoin fork? ##

In computer science, the term fork refers to the development of software based on the source code of a previous project.

In Bitcoin there are different types of forks: we consider **soft forks** , **Consensus hard forks** and **hard forks without Consensus**.

**Soft forks are made to introduce a new functionality to the Bitcoin protocol while preserving the retro compatibility of the new version.**

The most important soft fork of the last period concerns the introduction of SegWit (or Segregated Witness), whose main purpose was the resolution of the problem of malleability [21] of Bitcoin and that, as a secondary effect, &quot;streamlined&quot; the weight of transactions within the block.

There are no compatibility problems: non-SegWit wallets, whose addresses typically start with 1, can send bitcoins to SegWit addresses, recognizable because they start with number 3 or with bc1, and SegWit wallets can send BTC to non-SegWit addresses.

**Consensus hard fork**

Hard forks driven by the Consensus of the community are typically performed for the resolution of serious flaws in the code or for the introduction of a new feature not compatible with the previous code.

Let&#39;s assume that in the future will be necessary to increase the size of the Bitcoin blocks to increase the scalability on blockchain, ie the number of transactions for each individual block. Those who propose this change will seek to obtain the Consensus from the network nodes.

The change could initially be welcomed and the developers could write new versions of the software containing this increase in block size (eg a new version of Bitcoin Core).

Now the &quot;vote&quot; passes into the hands of those who maintain the nodes: if they accept the change, they will install the new version of the application, otherwise they will continue to use the current version, rejecting it.

When the nodes start installing the new software, the &quot;right to vote&quot; passes to the miners.

A date will be established in which the changes will become operative and the miners will have to choose which chain to mine: either the main one, without modification, or the new fork. The chain that will gain more computing power will be considered the main one.

If therefore the fork will have the support before the community of developers, then of the nodes and finally of the miners, then it will have gained the Consensus and called &quot;main chain&quot;.

It goes without saying that if one of these &quot;entitled to vote&quot; were missing, the fork would fail.

**Hard fork without Consensus**

Technically speaking, a hard fork without Consensus does not exist and is simply defined as a failed fork.

In fact, only the bifurcations that took place successfully, and therefore in agreement with the Consensus, are defined by the developers as &quot;Hard Fork&quot;.

**Nodes have the highest level of importance in Bitcoin**: if a hard fork is supported by the miners but rejected by the majority of nodes, it is highly probable that the bitcoin asset of the original chain would maintain a higher economic value than that of the initially longer and with more computing power secondary chain. The decrease in the new chain&#39;s bitcoin value would have repercussions on the miners, who would have less profit to continue to mine this blockchain and would therefore be forced, for economic interest, to shift their computing power over the previous one.

A recent example occurred with a Bitcoin Cash fork, also a Bitcoin fork that took place without Consensus. The new chain called BSV initially had more hashrate (computing power) than the old BCH (Bitcoin Cash) and its chain remained the longest for a few days. The majority of the Bitcoin Cash nodes however did not support the new fork and this led to a significant decrease in the price of the new BSV assets, with consequent huge economic losses on the part of the miners.

Now the Bitcoin Cash chain is again the longest, has more hashrate than that of BSV (more than double) and the asset has a market dominance of about 2% against 0.9% of BSV.

Clearly both these forks, having taken place without Consensus, do not represent the main Bitcoin chain, whose BTC asset has a market dominance of about 70%.

We said that Bitcoin is an open source project and that anyone can use the code for many different purposes.

We have also said that when the Consensus is not respected and the modifications to the protocol are carried out anyway, these, despite being rejected by the majority of Bitcoin nodes, create a fork to the code, called hard fork without Consensus.

What does this mean for us Bitcoin supporters (the main chain) and for our bitcoins?

Absolutely nothing.

The original chain is not affected by the changes and our bitcoins remain safe.

What happens is that the chain splits, a new chain is generated and this continues its path independently of Bitcoin.

It may happen that, if the modification project involves the creation of a new chain in competition with the previous one, a new asset is created: in the case of the non-Consensus fork of 2017, the bitcoin cash asset (BCH) was created.

Bitcoin holders suddenly found themselves in possession of two assets: bitcoin (BTC) and bitcoin cash (BCH). The first maintained its economic value, the second lost value compared to the first.

However, users had the opportunity to decide whether to keep both assets, sell one in favor of the other or simply ignore the second.

Personally I decided to support only the main chain and to respect the Consensus, so I sold my few BCH satoshis in favor of my precious good satoshis (BTC).

<img src="images/giacomino2.jpg" width=200 alt="Giacomo Zucco"> 
Giacomo Zucco&#39;s note: &quot;The analogy with a vote, however suitable to provide an understandable image of the complex dynamics of Consenus to non-expert readers, is certainly simplistic and should not be taken too literally. 
The choices made in the software development phase do not take place through a &quot;democratic&quot; vote, but with a complex merit-based process similar to those typically adopted by many open protocols (for example the Internet itself), based on concepts such as the &quot;rough consensus&quot; and described in part, for example, in the article by Jameson Lopp "Who Controls Bitcoin Core?" [22].
Even the so-called &quot;vote&quot; of the nodes should not be considered as such in the literal sense, for example due to the fact that the mere &quot;number of nodes&quot; does not represent a verifiable metric (the true metric, which can only be reconstructed ex-post and is not strictly quantifiable, concerns the economic weight of an institution that receives funds using a Bitcoin node for validation). 
Finally, even the so-called &quot;vote&quot; of the miners, as far as the relative hashrate represents, unlike the &quot;number of nodes&quot;, an objective and measurable metric, does not represent at all a &quot;democratic&quot; decision process, but is instead properly intended as a &quot;signaling of readiness&quot; mechanism, with purely technical connotations, even if there have been attempts to portray it as a &quot;political&quot; vote.&quot;
