## Appendix I - Best Practices ##

**Don&#39;t trust, verify!**
Always check that the software you use to manage your bitcoins does what it says it does. Prefer open source solutions instead of proprietary software, precisely because these can be tested by independent developers.

**Never share your private keys, for any reason and with any person.** Not your keys, not your bitcoins.

**Don&#39;t keep your wealth on a custodial wallet or any other third-party service.** You do not own private keys and the system is subjected to the issues of classic centralized systems. Transfer the your funds to an offline wallet (cold wallet) carefully stored and protected from external attacks.

**Stay away from the Get-rich-quick schemes** , in which someone promises you strong earnings and in a short time: these include the famous Ponzi schemes (or pyramid schemes), in which enriching ones is who is at the top of the pyramid and exploits the investments of who is below, promising them substantial profits but actually redistributing only part of the money coming from the new affiliates.

**Never invest more than you are willing to lose.** It is valid for any area, not only for a new technology like Bitcoin.

**Remember that Lightning Network is a still experimental technology** that could still have many critical bugs. If you want to test its features make sure you use a few satoshis.

**Consolidate the outputs of an onchain transaction**
With the increase in the value of the single bitcoin and the reduction of premiums for miners due to halving, it will be increasingly difficult to execute blockchain transactions that move few satoshis: the price of the fee may be greater than the total amount transacted.

The bitcoins on an address that cannot be moved because the commissions are greater than the same, are called dust: they can be the result of change or satoshis &quot;collected&quot; in microtransactions.
 Imagine that a user has several bitcoin addresses - which is common if you use a deterministic hierarchical wallet - and that many of them are dust.
 The user could have a significant amount of satoshis if he sums up all these funds but is not able to use them!

So here is the need to consolidate transaction outputs.

In times when the mempoils are almost empty it is good practice to collect all these dust and send them, in a single transaction, to an address belonging to us. Dust (the outputs) will therefore constitute the inputs of a single transaction that constitutes the actual balance sheet of the user.

In Bitcoin Core the procedure is quite simple:
 prepare a new outgoing transaction and select the reception wallet (one of your own, even inside Bitcoin Core). Then click on Coin Control - if you don&#39;t see the button you have to activate this function through the general settings - and select all the various outputs.
 Now in the Amount field you enter the maximum available, net of the fees you wish to pay.
 The various outputs will consolidate and, when funds arrive at your receiving address, you will see a single one in Coin Control.
 If you want to consolidate the funds on your light wallet, the procedure is just as simple: just send yourself the maximum amount (max amount), always remembering to establish the fees you wish to pay first.
 This technique is therefore useful in view of a future increase in Bitcoin fees, but consider that it could lead to a privacy problem, especially if you use an address previously used in the past or if the funds do not pass through a mixing system.

If on the one hand consolidating the outputs allows for lighter transactions and therefore less expensive in terms of commissions, on the other it exposes to privacy problems .

Let&#39;s imagine consolidating all our 0.01 bitcoin wallet outputs and having to spend, as before, 0.001 BTC for the purchase of a good or service: the seller will not see only 0.0015 BTC as in the example above. , but he will be able to know the entire balance of our wallet, because to make the payment we will have to send all our money (a single UTXO) of 0.01 BTC and receive the rest.

If we made a parallelism with bank transfers, it is as if the shopkeeper who has to receive a transfer, sees our entire balance instead of just the requested amount.

Therefore, remember this compromise when you want to consolidate your outputs and, possibly, divide your wallets: what you use for expenses (hot wallet) should always be different from what contains your savings (cold wallet).
