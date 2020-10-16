## What are the other possible uses of the Bitcoin blockchain? ##

The Bitcoin blockchain was created with the express purpose of establishing a transaction log, or rather a ledger of validated blocks containing transactions, which would allow all participants to keep track of their funds, avoid (or try to avoid) double spending of the latter and have an independent time reference.

**To avoid double spending and to agree everyone on who has what.**

Its function is therefore to certify that a certain transaction has taken place in a specific point in time and that it can be used only by those who own the private key relative to the public address to which the funds of that transaction are destined.

For this reason, one of the first names given to this block chain was time chain (or timechain).

Extremely, the blockchain is nothing but a register that changes over time and does not come back (or at least should not), not a revolutionary technology.
**The revolution is in HOW this ledger is updated and by WHO.**

Bitcoin, intended as a base layer and the set of protocols also containing the blockchain, in addition to all the other technological innovations that we have described above, is the real revolution.

Often those who use the term we are talking about do so out of context and therefore think that anything and every data can be put into a blockchain: from personal information to products information, from the results of an election to the algorithms that make an AI, or a car, work.

Basically a blockchain is used to carry data regarding monetary transactions. It is precisely the monetary incentive to make the system work, and the highest possible incentive is represented by the bitcoins that circulate in it.

What incentive would you have to install on your PC a useful program to make a decentralized network work if not the monetary one? Certainly there are those who would be willing to maintain a decentralized network for academic or civil interest, assuming that there was a decentralized network for scientific research or electronic voting, but the number of participants (also called &quot;nodes&quot;) would be clearly smaller than the ones in Bitcoin.

Having said that, which I repeat as a mantra to those who speak to me about &quot;The Blockchain&quot; and/or exalt it ignoring Bitcoin, let us now see what other possible uses this register could have.

Does the fact that the data is transaction information imply that it is not possible to use this register for anything else?

Absolutely not.

A transaction is made up of a series of information: in addition to the amount of bitcoins that are sent and those that are received as a change, assuming that it is a basic transaction from one address to another such as that seen previously between Alice and Bob, there is another parameter called OP\_RETURN: within this parameter we can insert information (limited).

Why should we need to insert non-monetary data on a decentralized system like Bitcoin?

In short, for safety reasons: security of conservation, non-tampering and non-censorship.

It&#39;s not to get that data to its recipient as soon as possible, since the block containing the transaction, which in turn contains this additional information, must be processed by all nodes on the network.

Secondly, to avoid building a new blockchain for each new use case, given that there would probably be servers deployed in the hands of a few actors (permissioned) or an effectively decentralized (permissionless) network but not as safe as Bitcoin&#39;s.

If you remember we said that, to ensure the highest level of decentralization, it is necessary among other things that the registry is as light as possible: it follows that the data that we could insert in the Bitcoin blockchain will be relatively few compared to those that other distributed ledgers may contain, but will make them poorly decentralized.

So **the choice is between safety and performance** , intended as speed and storage capacity.

When my niece was born I inserted the message &quot;_date XXXXXX, 22.00, Arianna was born!_&quot; in the Bitcoin blockchain, in order to have a memory of that day in the future. Several blocks have passed since then, so I can say with relative confidence that this message will remain forever in the shared ledger.

I used the Bitcoin network to transmit a data not related to a monetary transaction.

The fact of having entered this message in the blockchain, however, does not mean that it corresponds to the truth!

I could have written a different date than the birth date, a different name or other conflicting or non-relevant information.

This message constitutes useful and real information for me, and is therefore a totally subjective certification.

When we write in the Bitcoin blockchain data other than monetary transactions, we simply go to insert a record and protect it from changes over time caused by external agents (a central body, an attacker, etc.). **We certify the data, but this does not mean that the information entered corresponds to reality.**

We therefore understand that the blockchain, even if it is useful to protect the digital data from future tampering, does not guarantee its truthfulness and therefore does not lend itself well, for example, to the control of a supply chain.

Do we want to insert the serial number of a car on a blockchain?

Let&#39;s do it, but remember that there will always be someone in charge of writing that data and therefore it will be able to tamper with the reality: in short, the sedan car drawn on the blockchain, could prove to be a beetle after the delivery.

This is because it is not an object of the material world but a digital counterpart to be transmitted on the distributed ledger. Someone will have to create this digital object, right?

**Is the blockchain used for non-monetary purposes useless?
 No.**
 There is also the possibility of creating objective certifications if the &quot;timechain&quot; property is used to fix a data over time for something that actually requires a so-called timestamp; in short, if it is used as a timestamp register.

In this case the certification is not provided by the entered data (subjective parameter) but by the time it was entered in the blockchain (objective parameter).

**A practical example**

Soundreef is an independent copyright manager (Independent Management Entity according to EU Directive 2014/26/EU) recognized by the United Kingdom Intellectual Property Office[23], in competition with SIAE (Italian Society of Authors and Publishers) that in Italy, until recently, had a monopoly in the management and collection of copyright.

Well, from November 2018 Soundreef uses the Bitcoin blockchain to certify the authorship of the songs composed by its artists.

Soundreef authors can use proprietary software to obtain a digital ownership certificate: this is associated with a unique **hash** that is inserted into a Bitcoin transaction, thus ending up in its blockchain.

If someone were to plagiarize, the original author could prove ownership of the song simply by retrieving the certificate that was temporally marked.

Let&#39;s take a specific example.

I am an author and I have the file (the digital certificate) of my work dated November 1st, 2019 and the associated hash inserted in the blockchain the same date. If someone registered a plagiarism, this will be given later to my digital certificate/hash couple on blockchain, therefore, in the legal venue, it will be easy to prove the violation of my intellectual property.

The same thing can happen in the case of registration of patents, and in all those areas in which to count is the first to register the idea; where therefore a &quot;recorder&quot; or &quot;time marker&quot; is needed.

It is not necessary to use a proprietary software, as in the example of Soundreef, but it is enough to create a digital document in whose metadata the creation date is present, generate a unique hash corresponding to that document and write this hash in the OP\_RETURN of a Bitcoin transaction. It goes without saying that it is necessary to keep the original file and the corresponding hash. Without one of them we could not claim our property on the document, or rather, have it created and certified at a specific point in time.

**To date, the only function of the blockchain other than monetary transactions is the temporal marking of a digital data, or temporal certification (timestamp).**

Any other use is at least not appropriate, if not even fraudulent.

The famous &quot;supply chain tracking&quot; falls into these inappropriate uses and lends itself well to fraud.

**The example of the apple**

We have a NON-unique material object, an apple, which is &quot;digitized&quot; by a worker.

An Italian farmer sells its apples grown in compliance with the EU regulations to a large international distributor.

The distributor has business with many farmers and manages sales to shopping centers around Europe and North Africa. The products come from many different areas, some from the EU, others extra EU.

The distributor however uses &quot;the Blockchain&quot;!

The procedure is relatively simple: some workers collect the apples from the producers and apply a label, on which there is a QR code, on the cassettes. Other employees create digital objects containing information about the apples: date of harvest, origin, type of apples, etc. The QR code links these apples to the digital objects created by the workers and these are &quot;inserted&quot; into a blockchain (the marketing sector would say &quot;within the Blockchain&quot;).

If in the meantime the employer has replaced the boxes of apples produced in Italy with fruits produced in Morocco, removing the stamp from the Italian boxes and applying it on the Moroccan ones, it does not matter: when we will present ourselves in front of the fruit counter of our trusted supermarket and with the smartphone we will scan the QR code, we will be happy, because we will know that our apple is the one produced and harvested in Italy.

Shout out to the supply chain tracking through the blockchain!

I would like to point out that I have nothing against Moroccan apples, which could be even better than Italian ones. They are simply not the same thing and in the illustrated example a food fraud is carried out.

Why did I specify &quot;NOT unique object&quot; at the beginning of the example?

Because in fact this is the only case in which the &quot;transformation&quot; of a material object into a digital object and consequent tracking through a blockchain, could work.

If it were possible to describe in detail the physical-chemical characteristics of a single object to the point of realizing a digital counterpart of it, then we could be sure that the object in front of us is actually the example traced using (also) a blockchain. However, this is a fantasy, as the &quot;description&quot; of the single object is susceptible to human error.

Let&#39;s take a painting by Leonardo: we can describe the features that make it unique with very high precision. We can take this data, associate a hash with it and put this into the Bitcoin blockchain.

However, if our analysis turns out to be fallacious and a fake appears that corresponds to the characteristics expressed by our analysis, the digital alter ego would represent the wrong painting and the tracking would go to hell.

In short, as long as we remain in the digital realm and use the Bitcoin blockchain as a time marker (for example the ownership certificates associated with a hash) then we make an alternative but useful use of it, if instead we move to the real world, we can do nothing but &quot;track&quot; a digital object while the real one could be counterfeited or not be original, in case of unique objects.

Bitcoin&#39;s detractors tend to consider the inherent limitations of its blockchain and its poor predisposition to alternative uses such as proof that Bitcoin represents a bad monetary system.

With gold you can do so many things, with Bitcoin you can&#39;t!

The fact is that Bitcoin was created with the express purpose of establishing an alternative monetary system. It has precise features and functions.

If over time we will find alternative functionalities to the simple exchange of value among peers without a reliable third party, it is not known and is not even important right now.

Gold does not owe its value to the alternative uses that can be made of it, but to its scarcity which makes it a good Store of Value; it has been a precious metal for centuries, even before discovering its electrical conductivity and opening the field to its many uses in the technical/scientific field.

Some populations of South America, before the arrival of the European conquerors, possessed large gold reserves. Gold was mainly used as an ornamental material because it was malleable, resistant to corrosion and above all ... brilliant.

He had no monetary value among these populations, simply because it was not a scarce commodity. Pre-Columbian societies gave gold only a symbolic power mostly associated with the divinities of the Sun and, unlike Europeans, did not conceive it as a medium of exchange.

It is therefore clear that the value given to a good is completely subjective and extremely correlated to its scarcity.

If gold were not a scarce asset, its secondary uses would remain and perhaps increase in number, but its usefulness as a Store of Value and monetary medium of exchange would be lost.

Fortunately Bitcoin was designed to remain scarce and have the characteristics of a digital monetary medium.

<img src="images/giacomino2.jpg" width=200 alt="Giacomo Zucco"> 
Giacomo Zucco&#39;s note: &quot;To date it is actually possible to obtain a &quot;certain date&quot; certification (&quot;timestamping&quot;) even without writing ANY additional data on the Bitcoin time-chain, but by manipulating the data already entered for a normal transaction. 
For example this is possible with the technique called &quot;pay-to-contract&quot; (in which a public key is manipulated to insert a commitment to a message), or with the one called &quot;sign-to-contract&quot; (in which one manipulates a signature). 
The first technique is the heart of all future Taproot-related innovation, as well as being the one we use for the RGB protocol. 
Both can be used as a &quot;zero blockchain-footprint&quot; alternative to the more traditional OP\_RETURN, even in the context of the OpenTimeStamps library.&quot;
