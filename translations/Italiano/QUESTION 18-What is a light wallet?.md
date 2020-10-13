## What is a light wallet? ##
Unlike a full node which, as mentioned, downloads all the blockchain or at least all the transactions of our addresses and keeps them in memory, an SPV client only downloads the headers of the blocks, not the part of data that concerns transactions.

I will briefly illustrate the structure of the block here, inviting anyone interested to learn more, to read Antonopoulos&#39; Mastering Bitcoin.

If you find the text too complicated you can safely skip it and come back later, when you feel ready.

A block is divided into four major sections: **Block Size, Block Header** , **Transaction Counter** and **Transactions.**

For the moment it is enough to know that the &quot;weight&quot; of the block on the blockchain is mainly due to the transactions and, to a much lesser extent, to the Block Header. Transaction Counter and Block Size together occupy 5 to 15 bytes, a negligible amount.

Considering that on average in a block there are about 1500 transactions[24] whose weight is about 500 bytes each, while the block header takes up about 80 bytes, we deduce that, avoiding downloading transactions, you have a savings of considerable space, less than about 1000 times!

When needed, the SPV client verifies the transactions by relying on full nodes. We have said that the saving in terms of space is considerable, but this lower consumption of resources also involves a problem: the SPV wallet must indeed &quot;trust&quot; an external node, hoping that the node is updated and that it respects the rules shared by the network.
 The SPV wallet cannot independently check all transactions and therefore cannot verify that a Btcoin transaction has not been performed twice from the same address.

I know I&#39;m frightening you a bit, but it is necessary to understand that, when moving large funds, it would be better to do it through your own full node, while for small figures, you can tolerate the risk and rely on a light wallet.

For this reason, the most common type of wallet today is precisely the SPV, also due to the increasing use of smartphones to manage daily Bitcoin transactions.

There are many SPV wallets, more or less complete, in a number decidedly greater than those full node.

I will list some but this list is incomplete and does not consider hardware wallets.

**Desktop Wallet**

- **Electrum** : the best known SPV desktop client. Recently a malware version of Electrum has prompted users to display their private keys, so download the wallet always from reliable sources (the Electrum website) and beware of imitations.

- **Wasabi** : a client developed in order to substantially increase transaction privacy and therefore bitcoin fungibility. Wasabi wallet uses a technique called CoinJoin, which combines many transactions from different addresses into one big transaction, and this makes it extremely difficult to link senders to recipients.

**Mobile Wallet**

- **Edge Wallet** : open source multicurrency wallet produced by Airbitz Inc. I actively collaborate with this company, therefore, in full conflict of interests, I highly recommend it.
 Seriously, it&#39;s also a non-custodial wallet, so it allows you to export but also import private keys, and these are not managed or even seen by Edge creators (zero knowledge system). With Edge it is also possible to set customized Bitcoin nodes, which will be used by the app in order to download the Header. You can also use the full node you have on your PC.

- **Samurai Wallet** : a privacy-oriented mobile wallet for Bitcoin, with a very interesting function: the ability to send bitcoins offline, using an open source system for encapsulating transactions within text messages and messages sent on the txTenna mesh network. Samurai also has its own transaction mixing system, in order to increase user&#39;s privacy.
