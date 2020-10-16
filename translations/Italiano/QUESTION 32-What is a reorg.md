## What is a reorg? ##

Bitcoin is a technology created to allow digital monetary transactions between two entities without relying on reliable third parties.

To do this it uses, among other things, a chain of blocks in order to keep track of transactions and to prevent someone from spending the same money twice.

We tend to think that the blockchain is an immutable ledger and this idea has spread to the point of assuming systems that make use of it without resorting to some kind of monetary transaction.

The idea has even spread that the concept of immutability applies to any blockchain, regardless of the number of nodes, the mining algorithm used (PoW, PoS, DPoS, etc.) and the &quot;power&quot; made available by miners and validators.

In fact, **no blockchain is immutable**, not even the Bitcoin's one.

Immutability is a characteristic that we tend to, never reach it at all: the way in which we try to approach it is what allows us to distinguish a functional, useful or useless blockchain.

Bitcoin is the most technically secure chain of blocks and therefore the one that most tends to be immutable.

Besides the (tendency to) immutability, another parameter to consider when looking for a functional timestamp block system (aka blockchain) is its neutrality, its agnosticism, as mentioned in the chapter _Comparison between TCP/IP and LNP/BP_.

So: **neutral technology, tending to immutability**.

Neutrality is achievable when the rules of the game are established before the start and do not change during the game, in fact they work to keep them tight, just like a referee does during a soccer match.

The referee, in the case of Bitcoin, is the code. But let us remember that this is written by human beings, who are fallible and make mistakes, so it may be necessary to put the code to hand in order to preserve the initial rules, making the code work as it should.

In some cases the &quot;immutability&quot; of the Bitcoin blockchain could be put at risk by a voluntary (or &quot;coordinated&quot;) reorg.

A **reorg** is a common event for Bitcoin, to say the true, when it is not due to the will of an attacker: with &quot;reorg&quot; (or reorganization of the blockchain) we usually mean the event in which a client discovers a new correctly formed and longer blockchain than its reference chain and excludes one or more blocks that the client thought were part of the main blockchain. These excluded blocks become **orphans**.

In essence: I have a Bitcoin full node on my PC, my client realizes that the blockchain it is following is shorter than the one followed by the majority of nodes, so it stops following it and goes to the longer one. Consequently, if the one that followed has received transactions after the split, these will be considered invalid.

If you remember we talked about a similar event in the chapter _What happens to the miners who lose the race?._

In that chapter it was said that the miners receive the block containing the solution provided by the miner who is supposed to be the winner and verify it, like all the other full nodes.
 If the block is valid, they immediately stop working on the solution to the previous problem and start working on a new problem, contained within this new block.

If, however, they do not notice in time the presence of a valid solution, they will continue their work on the current block.
In this case, it may happen that a miner discovers the solution after the first miner; he will send its candidate block to the network and it will be rejected. His client will realize that he has mined on a shorter chain, because the main one has meanwhile gone ahead and the miners have started working on it.
He will therefore accept the defeat and will understand that the bitcoins that he has awarded as a prize are not valid, as are the fees contained in the transactions inside his block; the block he discovered will become an &quot;orphan&quot; and he will start working on the longest blockchain.

However, it may happen that someone tries a voluntary reorg of the chain, in order to invalidate transactions and assign bitcoins that are not due to him.

Take this situation in which every reference is purely coincidental: an exchange we will call &quot;Finance&quot; suffers the theft of a few thousand bitcoins, due to its inefficient security measures.
These stolen bitcoins are used by the hacker for many different reasons: buying a Lambo, paying for coffee, keeping them for the future.
In short, they are part of the system and are used in some transactions.

The owner of Finance, this BhangQeng Vhao (BV), gets a suggestion from a programmer who has worked on Bitcoin:
&quot;_if you reveal your private keys for the hacked coins (or a subset of them) you can decentralized-ly at zero cost to you, coordinate a reorg to undo the theft_.&quot;
BV thinks it is a good idea to modify the entire network ledger to cancel the theft and repair an error made by its exchange.

Big deal.

Technically it is possible: he needs to convince the majority of the mining pools, and therefore of the miners connected to them, to work on an alternative blockchain to the main one. The miners should begin to mine the shorter blockchain, the one in which the bitcoins were not stolen from Finance and moved by the hacker.

In short, they should rewrite history.

Of course, to do so they should have some economic incentive. Some miner should in fact renounce the reward obtained thanks to the blocks following the theft, plus all the transaction fees.

Let us imagine that the theft occurred at 8.00 am and that BV proposes the reorg at 12.00.
Four hours have passed, approximately 23 blocks from what we consider as block 0, the block containing the &quot;theft&quot; transaction.
Miners, after the block 0, obtained 287.5 bitcoins, without considering transaction fees.
If the single bitcoin is worth 10,000 USD, it means $ 2,875,000 in rewards.
For a reorg that cancels the thief&#39;s transaction, the block that contains it must also be reorganized, so the miners have to work on 24 blocks, giving up 300 bitcoins, excluding fees, or a value in USD of 3 million.

BV must hurry to convince the miners: every 10 minutes a block is added to the chain, so the costs increase rapidly!
It is logical to think that the owner of Finance could take a few days to organize a global reorg event: even if he has the possibility to contact the mining pools directly, it is a matter of making sure that the miners who support it are actually favorable to this initiative. Everyone would see their compensation canceled, and would remain with the sole hope that after the reorg the mining pool will distribute the new rewards.
If a few days pass, as is actually probable, BV should convince the miners with an incentive of a few thousand bitcoins, perhaps even higher than what was stolen from its exchange!

Let&#39;s imagine that he succeeds and that he convinces the vast majority of the pools to mine a version of the chain without the &quot;theft&quot; transaction.

The single bitcoin, the asset of a monetary system that is no longer resistant to censorship, would lose value drastically: the systemic (economic) crash would lead the miners to remain with a handful of useless digital collector&#39;s items.

Therefore they would have given up bitcoins obtained with extreme effort, useful to repay the expenses they sustained in terms of electricity for work and for the dissipation of the generated heat, wear and tear of the machinery, employees, etc. and to make a profit, and in return have obtained bitcoins which are always valid but which by now are unlikely to have an economic value because the system has lost one of the basic characteristics to which it has always tended, the non-reversibility of transactions.

**So any reorg is bad for Bitcoin?**

We have said that technology is designed to be neutral and prone to immutability. We have also stated that the referee is the code and not the will of the individuals who intend to change the system for personal interests.

This code, however, being written by humans, may be somewhat flawed.

Imagine that an attacker finds an error in the code that allows him to create a few million bitcoins out of the thin air.
The rules of the game state that it is not possible to create more bitcoins than expected for each block, that this amount is halved every four years from the start of the &quot;game&quot; and that there is a limit to the creation of new coins (the famous 21 million bitcoins).

If a flaw allowed us to violate these initial rules then we would have a problem. The developer community will have to get to work and ensure that the code respects the rules for which it was designed.

Let&#39;s say the attacker actually applied his discovery and generated 40 million bitcoins, but they could also be 1 satoshi more than the expected reward. These bitcoins could be used to make transactions.
Is it right therefore to push for a reorg of the blockchain that cancels these transactions, after that a new code without bugs has been issued?
From my point of view, a voluntary reorg is always wrong but there are those who say that, in this case, it would be a &quot;restore to factory conditions&quot;, that is to a code that does what it was created for.
This would ultimately be an error to be corrected, not a subjective change, the result of a political choice.

Take the example of a card game: one of the players hides jokers up his sleeve and decides to play them when it suits him.
The cards are more than the initial ones and the rules are violated by a striker, even if ultimately the mistake is of the dealer who did not prevent the cheater from starting.

In the initial example, instead, it is an initiative that does not have to do with preserving the rules of the network but with personal interests that place the community in front of a political choice.

During the Bitcoin story several bugs have been discovered, three of which were very critical.
In 2010 a bug was discovered in block 74638 which led to the creation of 184,467,440,737.09551616 bitcoins to three addresses.
Five hours after the discovery, Satoshi Nakamoto released a patch (a soft fork) that was going to insert a modification to the network rules: any transaction with more than 21 million bitcoins would henceforth be rejected by the network.
At the time the single bitcoin had recently gained an economic value and there were no consequences for users.
In 2013 the blockchain split again due to another bug. The situation was restored to normal around 6 hours later and there was a single double spending attack against OKPay. In 2018, yet another critical bug was discovered by a Bitcoin Cash developer and communicated to the main Bitcoin Core developers, who released a patch after 5 hours.

The Consensus decided in 2010 to continue the chain whose economic rules were those originally established, effectively canceling transactions that did not respect the limit of 21 million bitcoins, and in 2013 to roll back to a previous version of the protocol. If those reorgs had not been realized, it is not possible to know what the consequences would have been in terms of future reliability of the system and economic value of the asset and if an attempt to reorg of this type happened now, we do not know what the consequences could be in terms of Consensus and value of the bitcoin asset.

Luckly, the two events took place at an early stage in the history of Bitcoin, in which the asset did not yet have an important economic value and in which the number of nodes was extremely small.
