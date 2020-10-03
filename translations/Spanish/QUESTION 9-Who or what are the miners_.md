## Who or what are the miners? ##
There are nodes that, in addition to verifying network transactions and making sure that the Bitcoin rules are respected, have another feature: they work for the system and, specifically, they transcribe these transactions into the shared ledger called blockchain, making them irreversible.

But what do they do exactly?

We have said that Alice sends a transaction to Bob but that this, before reaching it, is &quot;parked&quot; in the temporary memory of the first available node.

These special nodes, called **miners** , draw transactions put into this temporary memory and transcribe them into a list called candidate block. Each miner creates his list of transactions and his candidate blocks.

Transcription is the simplest part of the miner&#39;s difficult job.

The miner, in fact, takes part in a competition with other miners: the aim of this competition is to find the solution to a cryptographic problem that is difficult to solve but easy to verify. Extremely simplifying the concept - I invite you to read Antonopoulos&#39; Mastering Bitcoin for the details of the procedure - they look for a number, an extremely complex code to find, which is the solution to this problem.

They need very powerful and expensive machinery to find this number. They proceed by trial and error with a method called &quot;brute force&quot;; they calculate the first number, test it and if it doesn&#39;t go well they discard it, they calculate the second, test it and if it&#39;s not good they discard it, and so on. The difficulty in finding this single correct number is such that a miner can find it on average every 10 minutes!

Imagine having a mathematical problem in front of you: instead of solving it using standard formulas, you go ahead by trial and error, because there is no formula that can easily provide you with the solution.

It&#39;s like when our brain has to do with multiplication tables or powers: initially the difficulty is low to the point that we can proceed by automatisms and by memory, but when the numbers increase we end up proceeding by trial and error, adding or multiplying.

Once the correct solution has been found, the miner inserts it into the block under construction together with the transactions: the number is the proof that the miner actually participated in the tender and is called &quot; **Proof of Work**&quot; . Afterwards, it sends this block, now closed, to the network, so that it is verified by the other nodes.

Imagine the miner&#39;s Proof of Work and the verification by nodes as a mathematical equation.

Let&#39;s see a very simple example based on a system of equations:

y= 2x

4x + y = 12

It solves this way:

4x + 2x = 12 and then 6x = 12

x= 2, y = 4

We spent some time solving this equation - very little, to be honest -, but we take less time to verify it.

It will be enough to replace the two unknown quantities x and y with the newly discovered numbers within the initial system.

**So finding the proof of work is difficult, verifying it&#39;s easy**.

In addition to the proof of work and the transactions of some users, the miner also enters another transaction, this time a bit special: it is set up to send a certain amount of bitcoins to the address of the same miner, as a reward for the work done.

**Where do these bitcoins come from?**
They are partly new and partly made up of commissions paid by those who send a transaction. We will see later on what this means: for now we just have to understand that the bitcoins, assigned by the winning miner to themselves, are called **reward** and this is composed of new bitcoins ( **subsidy** ) and commissions ( **fees** ).

They are in fact assigned by the winning miner to himself.

**But how many are these new bitcoins?**

If the choice were free, the miner would try to assign himself the highest possible number of bitcoins while respecting only the total limit of 21 million.

Fortunately, the Bitcoin rules are strict and the allocation of new bitcoins is predictable.

At the beginning of the Bitcoin history, the miner could assign 50 bitcoins for each block. The difficulty in calculating the Proof of Work was very low, like a simple equation.

Consequently a miner with good hardware could find many PoW in one day and 50 bitcoins were assigned about every 10 minutes.

At the time the single bitcoin had no economic value and those who mined technically did it at a loss, only to keep the system working, out of altruism or out of conviction that the value of Bitcoin, and consequently of their bitcoins, would be recognized tomorrow.

**Four years after the network started, something changed.**

The number of new bitcoins assigned by the miner to himself was reduced by half.

Was this a self-imposed punishment?

No. The system is designed like this.

**Every four years, in fact, the number of new bitcoins that a miner can assign to himself is reduced by half:** in 2012 it became 25.

This so-called **Halving** reduces bitcoin inflation, or better, the Bitcoin issuance rate, and, as a side effect, it tends to increase the value of the single BTC, because the units become more scarce.

In 2016 the subsidy for miners went down to 12.5 per block, in 2020 it will be 6.25, in 2024 it will be 3,125, and so on.

**What happens if the miner assigns more bitcoins than are foreseen by the system?**

Very simple. The block would not be accepted; the nodes would consider it invalid because it did not respect the rules of the network.

You can&#39;t cheat.

**What if the miner assigned himself less bitcoins than they owe?**

It seems impossible, because the mining systems are automated, but this has already happened.

In 2011, a miner, known by the nickname of Midnightmagic, assigned to himself 49.99999999 bitcoins instead of 50 as a subsidy for a block he discovered [19].

That unassigned satoshi is considered lost forever, because no one can assign more bitcoins than those established by the network rules. If Midnightmagic had assigned himself 50.00000001 bitcoins, he would have invalidated the block.

Paradoxically, if the miners began to assign themselves less bitcoins than they deserve, the BTCs in circulation would be reduced and the value per unit would increase.

In short, to Midnightmagic and to all those who make certain mistakes we say: &quot;_Sorry for your loss, thank you for the deflation_.&quot;

**What happens to the other miners who lose the race?**

The miner who guesses the correct number, the solution to the cryptographic problem on which all the miners were working and competing, wins the chance to &quot;close&quot; the block, insert it in the blockchain with the benefits described above.

What do the other miners do?

The other miners are nodes too (or they rely on them), therefore they receive the block containing the solution and they verify it.

If the block is valid, they immediately stop working on the solution to the previous problem and start working on a new problem, contained within this same block.

The miner who guessed the answer to the previous riddle and proposed the new cryptographic problem does not know the solution and can therefore also participate in the new tender.

There is no possibility to cheat and insert in the block cryptographic problems of which the answer is already known!

**Can miners work together to share profits?**

Absolutely yes!

The mining difficulty is now very high. Miners need very powerful machines and in large numbers to be able to have some chance of finding the correct proof of work and getting the reward.

This necessity meant that Bitcoin mining became a real industry and large professional mining centers were created.

However, this does not mean that the non-professional user is cut off from the system.

For some years now, in fact, many amateur miners, in addition to investing a certain amount of money in the purchase of specialized mining machinery called ASICs, have decided to collaborate with each other, creating coordinated groups.

These groups are called Mining Pools: the node of the Pool receives, like all nodes, the block containing the cryptographic problem and its software divides the problem into many small packages that it sends to the various miners connected to it.

They process their part of the problem and send the results to the Pool. When a miner discovers the correct solution, the reward goes to whoever manages the Pool and this shares it among all the participants in a fair way, based on the power provided by each, in addition to keeping a part of the prize as a commission (fee).

Let&#39;s say I am a miner and participate in a Pool that has 100 participants and a 1% fee.

My hardware contributes 5% of the total power.
 If I find the solution to the cryptographic problem I get 5% of the reward to which the owner of the Pool has taken 1% as his profit.
 I prefer to mine along with others because I would never have discovered the solution by myself: I would have had to solve a problem that was too big and difficult, while cooperating with other miners I had to solve many smaller and simpler problems at a time.
