## What is Lightning Network? ##

Lightning Network (LNP) is a structure of **payment channels** opened between private individuals and/or companies and represents the scaling solution for Bitcoin; that&#39;s why we often called it also the Bitcoin&#39; Second Layer.

With Lightning we can potentially make hundreds of thousands if not million transactions for second and so reach any part of the World (almost) instantaneously.

&quot;Yes, and for free!&quot;

Not really.

We can transact on Lightning Network and we can do it for a really cheap fee per transaction: personally I never spent more then 10 sats in fees.

But this will not be the case for so long.

Before exploring why and what we can do, let&#39;s see a bit how Lightning Network works.

Each member of the network can create his own node, equipped with a wallet, in which he can keep a certain amount of satoshis, or he can rely on a custodial service, with all the criticalities that ensue.

When an user wants to send a payment to another person or service on the network, he can open a communication channel with it, within which the satoshis will travel, just as the data packets routed by the transport protocols, such as TCP, travel between the devices connected to the Internet. The discussion on the structure underlying the Internet is a bit complicated so we will go into it later.

<img src="images/lightning%20network-4.jpg" width="1000" alt="lightning network">

In the image on the previous page: the black arrows coming directly from the nodes represent blockchain transactions, while those inside the channel are Lightning transactions.
By convention, only three transactions are shown as directly related to the Bitcoin blockchain and are used to open two channels, Alice&#39;s with Bob and Alice&#39;s with Carl, and to close the channel that Bob opened with Earl. All other black arrows outside the channels also represent blockchain transactions.
Alice was able to open two channels with two different nodes through two onchain transactions.
Within the channels she can perform all the transactions she wants, without waiting for confirmations or paying fees to the miners.
Bob closes the channel he has with Earl and his satoshis are poured onto the blockchain through a single closing transaction.

<img src="images/lightning%20network-3.jpg" width="1000" alt="lightning network">

In the first image the two large panels symbolically represent the two layers: **Settlement Layer** , as the base layer (blockchain), and **Transaction Layer** (Lightning Network channels).

The representation of the most correct Transaction Layer should consider only the payment channels and not the transactions outside of them, but for reasons related to the simplification of the representation on levels, this solution has been chosen.

**Let&#39;s make it easy. How it works with an example.**

Imagine that you are in a group of five friends with a fixed appointment: friday night at the pub.
 Every time you go and drink and eat together, you go to the pub checkout and have your bill split so that everyone pays for what they have consumed.
 The owner of the pub will have to print more receipts, spend some time to collect the money from the individuals by increasing the line in front of the cashier, and be careful to reach the correct total. In short, this system is inefficient; it&#39;s slow, expensive, definitely not scalable.

Now let&#39;s assume that you and your friends want to do things more efficiently.

You calculate that each month you spend an average of 100 satoshis each.
 You could put these 100 satoshis in a common fund and keep each of you the bill on the expenses made.
 Once you reach the pub checkout you can pay the owner in a lump sum, knowing that none of you will lose out because you know exactly how much the individuals spent.
 From the following month, if Alice, a member of the group, spent 50 satoshis, she will integrate the common fund with 50 satoshis, if Bob has spent 20, he will add the same number to reach the 100 satoshis, and so on.

The common fund could also be useful outside the pub: if Bob wants to buy a pizza that costs 5 satoshis but has no money with him, he could ask for a loan from the common fund he has with his friends and integrate 5 satoshis at the next expense at the pub.
 On a pub bill of 20 satoshis each, Bob will pay 24 and all the others 19.

These extra expenses can take place a theoretically infinite number of times, the important thing is that each member of the group keeps track of the expenses and that each month everyone has a balance of 100 satoshis.

This is similar to what happens with the Bitcoin second layer called Lightning Network[32].

You and your four friends open a payment channel (in the example, the common fund) by executing a single transaction each on the Bitcoin blockchain. Instead of being a standard transaction, which requires a single signature to spend the funds, this is a **multi-signature** transaction. Multi-signature transactions are, in a nutshell, complex and programmable transactions, which allow different parties to participate. Individuals cannot perform outward transactions without the authorization (signatures) of the other participants.

The parties are anchored to the Bitcoin blockchain by a multi-signature contract and can now send transactions between them within the channel, without the need to transmit all to the blockchain. The channel requires funds to be inserted inside it: **it is necessary that at least one of the parties involved in the opening of the channel pay the funds**.

This money inserted in the payment channel is called **Channel Capacity** , that is the satoshis capacity of the channel just opened.

Channel participants keep track of the balance ( **channel states** ) and only send the last balance of the channel to the Bitcoin blockchain if they wish to close the latter.

So if Bob wants to get out of the common fund, he can do it: his debt to the fund will be calculated and he can take the satoshis left out of Lightning Network, back to the blockchain, minus the usual mining fee for the onchain transaction.

**A true P2P electronic cash system**

So now we understand that **Lightning Network is a structure of payment channels where users can exchange satoshis directly with each other, without a miner collecting their transactions and inserting them in a new block.**

The only mining fees you and your friends will have to pay will be those of sending satoshis to a Lightning node for opening a payment channel with it and those for closing the channel with consequent sending of the remaining satoshis to the Bitcoin blockchain, instead of all those deriving from the individual onchain transactions that you would usually do.

For each channel that you want to open a channel capacity is established: let&#39;s say that I have 0.01 BTC in my wallet, or 1 million satoshis. I could decide to open a direct channel with a friend of mine with a capacity of 20,000 satoshis, one of 100,000 satoshis with my favorite pub and many others. I will then be able to execute all the transactions I want using these channels without having to close them. The pub, on the other hand, may from time to time decide to transfer satoshis to its onchain cold wallet, just to keep important quantities offline and protected thanks to the (tendency to) immutability of the Bitcoin blockchain.

**Not just direct channels**

If Lightning Network would allow the transfer of satoshis only to direct channels it would be completely useless, or better, its usefulness would be only for recurring payments between two people and/or companies in direct contact. In reality this network allows to have what in jargon is called **Payment Routing** : I can send satoshis even to those who are not directly connected to me through &quot;jumps&quot;, called hops, between nodes.

Imagine that a friend has to pay for his beer at the pub but does not have a direct payment channel with the place.
 Instead of opening one, with the resulting fees to be paid and waiting time, because it would have to wait for confirmations of the onchain transaction, this reads the pub&#39;s invoice and pays: the satoshis will first pass by a channel opened by our friend with another person and will jump from node to node until they reach someone whose node has a direct channel with the pub.

In our example, if our friend has a direct channel with our node and we have one with the pub, it could happen that the satoshis will pass by our node first and then arrive at the pub&#39;s node.

The more nodes available to the Lightning Network, the easier it is to make these indirect payments. Few nodes mean a high possibility that the payment is not successful!

It is as if, in the material world, we had to pay a person who is in another city using banknotes: we can hand over the money to one of our acquaintances and this will deliver it to other people, until it reaches the real recipient.
 Obviously, although similar to an indirect payment system of the material world, here there is no danger that one of the participants in charge of delivering the money to the next will run off with the loot, because the network is based on **smart contracts** and not on direct intervention of people.

**Lightning therefore constitutes a true P2P network** , in full compliance with the abstract of the Bitcoin whitepaper created by Satoshi Nakamoto, while the Base (Settlement) Layer, with its blockchain, is more similar to a broadcast system, since the transaction transcription and so their irreversibility depends on the miners.


<img src="images/Scan0074.jpg" width="1000" alt="lightning network">

**The Lightning Network Fee Market**

Every transaction comes with a price. This is true for any kind of transaction, and if in the classic transaction layers (for example Visa or Mastercard) you don&#39;t pay fees, it&#39;s because someone is paying them for you: usually the store owner, that, if it&#39;s smart, will increase a little bit the price of its goods to cover the commissions.

This is also true for Lightning Network.

&quot;_Ok, but how much I need to pay?&quot;_

It depends.

If with a Bitcoin onchain transaction you pay a mining fee that correspond to the fees you want to pay multiplied by the size in byte of your transaction — you could potentially pay high fees for a transaction with low economic value and low fees for a high value TX (see Appendix IV, &quot;_How much does it cost to send bitcoins?&quot;_)_—_ , with Lighting you could have literally ZERO fees but you have other parameters to consider.

**Base Fee** : when you open a channel with a node, you should know what&#39;s the Base Fee it will require for every transaction that goes through it and reach another node.
 If the Base Fee is for example 1 sat, you will pay 1 sat as a fixed price.

**Fee Rate** : when you send a transaction, this go through a node and this has set a Fee Rate, you pay a percentage of the total amount as a fee.
 Fee Rate is expressed in mili mSats, so for example if a node ask for 1000 mili mSats as a Fee Rate, it will ask for 0.001 sats.
**You need to multiply this amount for your total amount**.

You want to transfer 2000 sats? you pay 1 sat (Base Fee) + 2000 x 0.001 sats (Fee Rate) = 3 sats as a fee (Base Fee + Fee Rate).

Is that all?

No.

You need also to consider the amount of hops your transaction will need to do!

If you don&#39;t have a direct channel with a node and you need to pay for a service, you will relay on another node and it will eventually do the same with another one, until the service&#39;s node is reached. We saw that before and we call it Payment Routing.

So, let&#39;s say Alice need to pay David — yes, more sats for me! — but doesn&#39;t have a direct channel with him.

Alice has a direct channel with Bob, Bob has a channel with Carol and Carol with David.

The transaction will need to go through 2 nodes!

So, let&#39;s say these node have the same Fee Rate and Base Fee: Alice needs to pay Carol too, not only Bob, so 2x the fees.

Now the 2000 sats for David will need 6 sats to go through.

As you can see, even if the fees are low (0.3% of the total amount), they are not zero.

**It&#39;s important to note that Alice can decide the max amount of fees she is willing to pay**.

If 6 sats are too high for her, she could select a smaller cap: let&#39;s say 3 sats.

Her node will calculate another route to David (if any) in which routing nodes require less fee.

Alice and David are both connected to Isaac, an LSP (Lightning Service Provider). This has a Fee Rate of 1000 mili mSats and a Base Fee of zero sats.

If Alice pays David 2000 sats, she will need to pay only 2000 x 0.001 sats (Fee Rate) = 2 sats.

She will pay the 0.01% of the total amount as a fee.

So, as you can see, if a user set a max amount of fee that he/she is willing to pay, the node will search for the best route with the lowest fee.

**The Lightning Network Fee Market is starting**

We can understand that node operators have two main options:

1. They could decide to keep the fee almost static and even high if compared to the average, in order to keep their channel balanced and sporadically earn some high routing fees.
2. They could follow (or better, create) the market and have dynamic fees so they can have more routing events, earn less per routing but have an overall bigger routing fees adding up all the transactions.

**What can we do to be active users and to keep the fees low?**

Well, first of all we should start creating node and opening channels.

**It&#39;s better to have many nodes that a lot of channels with a small network of nodes!**

Then, we should select good nodes in terms of capacity and availability, but we can also look at the Base Fee and Fee rate required.

In my case, I created a sort of price list for my routing services:

<img src="images/lightning%20price%20list.png" width="500" alt="lightning network">

So it&#39;s like I&#39;m selling my route service (or capacity) for a price: in this case I request zero sats as Base Fee and a variable Fee Rate that start from 1 mili mSat (0.000001 sats) and reach 2000 mili mSat (0.002 sat) if a user open a channel with 2 million sats of capacity to my node.

This price list will eventually change, adapting to the Lightning Network Fee Market, once the network will be bigger and there will be more competition between routing nodes.
