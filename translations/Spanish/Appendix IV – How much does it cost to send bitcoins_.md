## Appendix IV – How much does it cost to send bitcoins?.md ##

One of the myths about Bitcoin to dispel is related to the cost per transaction (mining fees).
Specifically, the myth is: _&quot; The higher the transaction amount, the higher the commission spend.&quot;_
This misunderstanding is probably due to what happens with classic payment systems, especially with cross-border payments: a commission is usually paid as a percentage of the transaction._

With Bitcoin, things work differently: you could potentially find yourself in the situation where transferring a billion dollars in bitcoin costs less than transferring a few USD.
Why?

When we transfer bitcoins, our wallet constructs the transaction, aggregating the quantities of available BTC.

Let&#39;s imagine our Bitcoin wallet as a classic cash wallet. Inside we have some 10 euro banknotes, some 20, some coins and so on, for a total of 130 euros.

If we had to pay for a good or service that costs 100 euros, we should obviously add up the various banknotes until we reach the required amount. If we exceed the amount and pay, we will get a change (if for example we pay with a 50 euro banknote and three 20 euro banknotes).

In Bitcoin the procedure is very similar: those previously defined &quot;amount of available bitcoins&quot; are actually called unspent outputs (UTXO) and become, all or part of the inputs of our transaction, that is the &quot;banknotes&quot; that will go to form the total transaction.
<img src="images/utxo.png" width="800" alt="UTXO">

_On the left, a transaction that uses a single UTXO as input, on the right a transaction that uses multiple UTXOs as input and transfers the total to a single output. Source: https://commons.wikimedia.org/wiki/File:Bitcoin\_Transaction\_Inputs\_and\_Outputs.png_

Let&#39;s imagine we have a total of 0.01 bitcoins in our wallet - or 1&#39;000&#39;000 satoshis, if we prefer to think with this unit of measurement -, equal to around 80 euros the moment I&#39;m writing. However, these bitcoins are the result of many unspent outputs, because we received about ten transactions of different amounts for them.

In the event that we have to pay for a good / service costing 100,000 satoshis (0.001 BTC), our wallet will take our &quot;cash&quot; and add them up to obtain a sum equal to or greater than the amount due.

Let&#39;s assume that the total sum is 0.0015 BTC and is the result of 4 UTXO added together: we will pay 0.0015 BTC, 0.001 BTC will go to the seller while 0.0005 BTC will return to our wallet, and will constitute a single unspent output.

Then, recap:

1. we had 0.01 BTC (balance sheet) consisting of a dozen UTXOs: 0.0002 BTC + 0.0007 BTC + 0.0001 BTC + 0.0005 BTC + ...
2. The wallet sums the first four UTXOs and gets 0.0015 BTC.
3. It pays this 0.0015 BTC to a seller, get back a single UTXO of 0.0005 BTC (change), which adds up to the other outputs that make up the total remaining balance.

A transaction consisting of many inputs has a weight in bytes greater than one with few or even a single input. **We do not pay based on the amount of bitcoins moved, rather it can be said that we pay based on the amount of unspent output that we are going to use as an input to our transaction.**

Commissions to miners are paid in sats per byte (or sats/vbyte for SegWit commissions).

Let&#39;s assume we want to pay 4 sats / byte because we are in a situation where there is no congestion in the Bitcoin network and we are pretty sure that our transaction will be confirmed within a few hours, becoming part of the transactional history of the transaction chain ( blockchain).

A good wallet allows, among other things, to manually set the commissions , so let&#39;s select 4 sats / byte and choose the amount to pay.

In Edge Wallet we can determine which commissions to use, choosing from High, Standard, Low or Custom. With this last option we can specify the fees in sats/byte.

Since we have a lot of inputs, our transaction will have an important weight and those 4 sats/bytes could lead to a relatively high total cost in commissions.

For example, if our transaction had a weight of 400 bytes, we would end up paying 1,600 satoshis (4 x 400 bytes).

Our 0.0001 BTC transaction will therefore have a commission of 1,600 satoshis (0.00001600 BTC).

Now let&#39;s imagine that we are a millionaire and want to transact 1,000,000 euros in BTC, or about 124.5 bitcoins today. If we had these bitcoins in a single unspent output, our transaction will have the least possible weight: let&#39;s assume 200 bytes.

With the same sats/bytes, therefore, this transaction will involve a commission cost of only 800 satoshis (4 x 200 bytes), compared to 1,600 satoshis of the previous one.

So with 800 satoshis (0.064 euros), we moved 1 million euros in bitcoin, while previously with 1,600 satoshis (0.13 euros) we only moved 80 euros.

In the first we spent 0.1625% on commissions, in the 1 million euros transaction we spent the 0.0000064%.

We therefore understand that moving 1, 100 or 1 million bitcoins makes no difference, as long as you have a transaction with the same weight in bytes.

How can we spend as little as possible on commissions?

First of all, as mentioned previously, we must choose a wallet that gives us the possibility to set a custom commission; therefore we discard all those who do not give us this possibility.

Another useful tip is to have a small number of unspent outputs within the wallet, but the latter does not always allow us to know which and how many UTXOs make up our total balance.

We can therefore decide to consolidate our unspent outputs into a single spendable output with the least possible waste of satoshi for transaction fees as we saw in Appendix I.

Consolidating the funds on your light wallet is quite simple: just copy a reception address and send the maximum amount to it, always remembering to first establish the fees you wish to pay.
