## What is the blockchain? ##

Technically speaking, **the blockchain is the ledger of validated blocks of the Bitcoin protocol.**

Now we need to go deeper, because it is a difficult concept to understand, since most of us are used to cash transactions in the real world and, when it comes to digital transactions, it is not clear how these happen.

Let&#39;s see together how digital transactions take place and how we arrived at the definition of blockchain mentioned above.

If you remember the example about the transaction between Alice and Bob, we said that in classic digital transactions there is a third party that authorizes the payment.

Well, what it does, in short, is nothing more than updating the internal register containing Alice&#39;s movements and sending the update request to Bob&#39;s bank, which will update the balance of the latter.

Therefore, there are no files (or tokens) transferred between one bank and another, much less cash transferred physically from one party to another by means of a delivery service.

These are pure and relatively simple numerical ledgers.

So, let&#39;s come to the blockchain, a register that do not need the reliable third party, and analyze it.

A very first definition of blockchain could be the following: a distributed and decentralized list of digital data inserted respecting a temporal order.

You will understand well that I have told you everything and nothing.

What data? A distributed list between whom? How decentralized? Which temporal order is and established by whom?

In short, such a definition raises more questions than answers.

**A distributed ledger**

The concept of distributed ledger ( **DLT, Distributed Ledger Technology** ) is very generic and refers to a technology that allows data to be stored in a distributed way, avoiding centralization on a single large server, which if attacked could lead to the fall of the entire system and the consequent loss of the data itself.

Distributed Ledger technology is decentralized in data management but does not necessarily imply decentralization of the organization that adopted or created it. Potentially, it can already be used by your bank.

**The chain of blocks**

The concept of &quot;chain of blocks&quot; (later become time chain, then block chain and finally blockchain), was introduced by Satoshi Nakamoto in 2008, in his document &quot;_Bitcoin a peer-to-peer electronic cash system_&quot;[CITATION Sat08 \l 1040]: to ensure that a completely digital monetary system could exist that could not be attacked by third parties, such as hackers, governments and private institutions, it was necessary to find a way to decentralize network management and the issuance of monetary units. It was also necessary that the new system did not allow the user to spend the same money several times, just as it is not possible for the same person to pay twice with the same banknote.

But I am repeating myself because we have already seen, in the first chapters, what Bitcoin is and why it was created.

So here is the idea of using a &quot;block&quot; validation system.

We have already seen that the block is created by a miner and is, in essence, the set of some transactions made by the users, a transaction that pays the miner for the work done and the Proof of Work he discovered.

But the block has something more inside it:

- **a sort of index that links it to the previous block**
- **the problem that the miners will have to solve and that will be linked to the next block.**

We simplify by imagining the block as the page of a book that has thousands more pages.

If this has not a page number and is removed from the book along with others, it would be difficult if not impossible to put it back in its place, to understand the reading order.

The blockchain is just like a book and the blocks, temporally ordered, constitute its numbered pages.

Through this book we can monitor all the transactions made by the participants, make sure that no one cheats, for example spending twice the same money, and even go back to the very first transaction, contained within the first block, called Genesis Block, made by Satoshi Nakamoto.

Side note but of fundamental importance.

**There is no blockchain without Bitcoin!**

The blockchain is only a part of the Bitcoin Protocol, which is the set of all the protocols and different technologies.

The base layer Bitcoin Protocol does not work without blockchain as it does not work without digital signatures, cryptographic keys, Proof of Work, nodes, etc.

However, we can exchange bitcoins (the currency of the system) even without resorting to the blockchain, or better, using that only for a small part, thanks to the so-called transaction layers, such as Lightning Network.

**The blockchain, in a sense, is inefficient by design**.

Its purpose is not to allow fast and free transactions but to ensure their irreversibility (or the tendency to irreversibility) and provide a temporal order to the blocks that contain them.
 Each block must be communicated and verified by all the nodes of the network, which complicates things with regards to scalability and speed of transactions.

<img src="images/libri%20blockchain-1%20A.jpg" width=400 alt="blockchain">

Furthermore, this ledger, being public, does not lend itself to the anonymity of transactions, since these are clear and visible to all participants.

When someone tells you that Bitcoin is chosen as a payment system by criminals because of its anonymity, it actually says something that is not true.

Bitcoin is pseudo-anonymous: the blockchain keeps track of the Bitcoin transactions and addresses involved. They are, as mentioned, alphanumeric addresses and not names, so it is assumed that transactions take place anonymously for this reason. In reality, when a user makes his address public, he loses anonymity, unless he conceals his identity behind a nickname.

For example, if I need to receive a payment through the public address 39EVqFcspspQRgNKPuugsbGrn5NN5QvUT9 and I associate it with my name and surname, all transactions related to that address could be traced by anyone who wanted to carry out investigations.
