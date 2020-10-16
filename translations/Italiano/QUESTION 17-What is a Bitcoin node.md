## What is a Bitcoin node? ##

In IT, &quot;node&quot; indicates any hardware capable of communicating with other devices connected to the network.

In Bitcoin, things get a little more complicated.

Users can in fact interact with the Bitcoin network and each constitute a node by transmitting information relating to the transactions, even if in different ways.

There are different types of nodes, specifically: **full node, miner node** and **SPV client** (although some, including myself, struggle to consider these nodes).

Originally full node and miner node coincided. The miner needed to keep a copy of the entire Bitcoin blockchain in order to do his job and who, instead, just wanted to verify the transactions, could act on his node and disable the mining feature.

To coincide were not only full node and miner node but also the concept of node and wallet.

If at this point in the book you have clear how to store and send bitcoins, you will know that to execute transactions we need an electronic wallet.

The first ever wallet, which still runs on most Bitcoin online full nodes is the Bitcoin Core wallet, also called Satoshi Wallet, because it was developed directly by Satoshi Nakamoto. You can download it from the [bitcoin.org](https://bitcoin.org/) website or from the GitHub [repository](https://github.com/bitcoin/bitcoin).

Bitcoin Core is a full node software: to fully utilize it, you need to download the entire Bitcoin blockchain, which currently weighs about 250 GB. The blockchain can be downloaded in different ways: with the txindex disabled or enabled (txindex = 1), in Pruned mode or with this mode disabled.

What does it mean?

In Pruned mode, the user maintains a smaller version of the Bitcoin blockchain. The oldest data is deleted (eg old transactions not directly linked to your addresses). This means that you can save a lot of disk space: for example, we can decide to keep only 500 MB of data instead of the over 250 GB required by the entire blockchain.

If we download Bitcoin Core, we do not activate the Pruned mode and in the configuration file we insert the parameter txindex = 1, instead, we will download the entire Bitcoin blockchain plus the complete transaction index, that is the whole history of the transactions performed by the members of the network.

All of them!

Downloading the entire Bitcoin blockchain gives us a complete user experience that is perfectly in line with the philosophy behind the protocol: the possibility to completely and independently verify all transactions, without having to trust another node or other verification system, including the ability to influence the Consenus, because we could reject any changes to the Bitcoin rules by simply refusing to update the software to a version that contains them.

The verification is useful, among other things, to avoid accepting &quot;double spending&quot; transactions if the system has undergone a double spending attack or a hidden fork.

For the average user this can be an excessive precaution, but it allows you to actively influence the choices of the network.

Furthermore, for a company operating in the sector or for those who want to activate a Lightning network node, it is essential to have Bitcoin nodes that are always updated and contain the complete history of the network.

There are also other full node implementations, such as Bitcoin Knots, Libbitcoin or bitcoinj, just as there are different software for managing another decentralized network, used to share files rather than a transaction ledger: the BitTorrent network.

To guarantee decentralization of the system and its security, we should continue to maintain and develop different full node softwares.

As we have seen, a full node can weigh up to several GB, so it was necessary to develop solutions that would allow even those with limited resources, such as low memory capacity on the PC or poor Internet connection, or to anyone wishing to use mobile devices, to be able to manage Bitcoin transactions independently and without private keys &quot;custody&quot; by third parties.

For this purpose the SPV (Simplified Payment Verification) wallets, also called lightweight clients or light wallets, were developed.
