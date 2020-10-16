## What is a hardware wallet? And a paper wallet? ##
Let&#39;s start with the **paper wallet**.

We said that a Bitcoin wallet is composed of two series of numbers: a public address and a private key, with which transactions are signed and funds are set in motion.

The bitcoins you receive do not physically reside in your wallet (your app on your phone or your desktop software), or anywhere else.

It simply keeps track of the various owners, ie the public addresses to which the bitcoins that run in the system have been sent, on the blockchain.

It can therefore be deduced that, as long as we have the private key associated with an address on which we received bitcoins, we could use them wherever we are and with any application that allows us to import the keys.

If the app we use allows us to export private keys, we can make a backup of them simply by writing them on a sheet of paper.

If instead the application does not allow us to export them, well, we change app.

**A paper wallet is simply this: a sheet of paper or other medium on which we have written our private keys**.
 We will have to guard it carefully, away from prying eyes, because that sheet contains our wealth.

**Hardware wallet**

A hardware wallet is, as the name implies, a device that we can use in tandem with compatible software to confirm our transactions.

The device contains the private keys of our Bitcoin wallets: when we have to execute a transaction this is signed through our hardware wallet and the private key is never exposed.

If we use a hardware wallet, however, we must be aware that this tool is only an additional protection to our paper wallet.

In fact, during the configuration of the device, we will have to memorize on a sheet a series of words called **seeds**. These seeds make up our Master Private Key, so if we lose them we will no longer have access to our bitcoins in the event of a hardware wallet failure. As with the paper wallet, keep this sheet safe!

The most popular hardware wallets on the market are currently produced by Trezor and Ledger. Between the two companies I would recommend the devices produced by Trezor, because they have an entirely open source software; this gives the possibility to check that there are no backdoors in the private keys management system.

Ledger uses bank-level security systems, which effectively neutralizes some physical attacks against which Trezor cannot effectively defend itself, but at the cost of having an important part of closed code, that is not verifiable by independent developers and therefore potentially exposed to backdoors.

In addition to the two hardware wallets mentioned, Coldcard should also be considered, a very interesting hardware proposal that integrates a dedicated chip for storing the private key and provides the user with a &quot;duress PIN code&quot;, ie a security code useful in case of physical attacks: if typed, the wallet will not give access to the user&#39;s funds, but to another wallet, on which the owner could have uploaded only a few satoshis. The attacker would therefore not have access to the main wallet.

Another interesting feature of Coldcard is the so-called &quot;Brick Me&quot; PIN, which instead, used in extreme cases, destroys the private key and makes the wallet completely useless.
