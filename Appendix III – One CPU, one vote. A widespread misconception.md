## Appendix III – One CPU, one vote. A widespread misconception ##

&quot;One CPU, one vote&quot; is a widespread misunderstanding, due to a misinterpretation of the following statement by Satoshi Nakamoto, contained in the Bitcoin withepaper: &quot;_If the majority were based on one-IP-address-one-vote, it could be subverted by anyone able to allocate many IPs. Proof-of-work is essentially one-CPU-one-vote. The majority decision is represented by the longest chain, which has the greatest proof-of-work effort invested in it. If a majority of CPU power is controlled by honest nodes, the honest chain will grow the fastest and outpace any competing chains._&quot;

First of all, the above statement is often extrapolated and used out of context. Nakamoto was, in this case, describing how Proof of Work works (section 4 of the whitepaper), not the Bitcoin Protocol.

Let&#39;s take for good the fact that in Bitcoin there is a &quot;democratic vote&quot;, which is actually not true, as we have seen in the chapter _What is a Bitcoin fork?._

When Nakamoto elaborated the phrase &quot;One CPU, one vote&quot;, the conditions were as follows:

1) the only relevant case of Proof of Work applied to an electronic cash system was that of Hal Finney&#39;s RPoW, applied to his digital money project. Prior to this, PoW was simply used as an anti-spam system.

2) PoW used the CPU for brute force calculations: the more powerful the CPU the more calculations you could make. The more CPU you had available, the greater your weight (the so-called &quot;vote&quot;) in the Proof of Work system.

3) No one had yet used GPUs nor invented the ASICs, so Nakamoto linked the increase in the mining difficulty ONLY to the increase in the number of CPUs and to the performance of the latter (Moore&#39;s law).

4) Full node were validators but also miners. If you didn&#39;t want to mine with your hardware, you had to disable this feature.
 To date, the miners are not validators (due to Stratum V1), but will again be able to do so in the future thanks to Stratum V2 (see chapter _What are the main critical points of Bitcoin?_). In any case they would not have a greater role in the Consensus but would extend the mining decentralization.

5) Miners do not have a prevalent role on the Consensus but are at the service of the validator nodes. For this service they receive a monetary incentive consisting of subsidy + fees (reward). In the case of a hard fork they adapt to the chain that has Consensus because they are driven by profit, not by goodness or democracy.
 To understand why they have no decision-making power, see the case of Segwit2x (from a proposal supported by large mining pools) and the lack of adoption of this proposal by the community.

As we have said, however, with the phrase &quot;one CPU, one vote&quot;, Satoshi Nakamoto was referring to a single component of Bitcoin, the Proof of Work, and not to the entire operation of the system; therefore the conditions expressed above are completely superfluous in that context and only serve to understand that applying this sentence to the entire Bitcoin Protocol is incorrect.
