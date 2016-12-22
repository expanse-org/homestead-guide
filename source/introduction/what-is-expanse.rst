.. _what-is-expanse:

################################################################################
What is Expanse?
################################################################################

Expanse is an open blockchain platform that lets anyone build and use decentralized applications that run on blockchain technology. Like Bitcoin, no one controls or owns Expanse – it is an open-source project built by many people around the world. But unlike the Bitcoin protocol, Expanse was designed to be adaptable and flexible. It is easy to create new applications on the Expanse platform, and with the Homestead release, it is now safe for anyone to use those applications.

================================================================================
A next generation blockchain
================================================================================

Blockchain technology is the technological basis of Bitcoin, first described by its mysterious author Satoshi Nakamoto in his white paper "Bitcoin: A Peer-to-Peer Electronic Cash System", published in 2008. While the use of blockchains for more general uses was already discussed in the original paper, it was not until a few years later that blockchain technology emerged as a generic term. A blockchain is a distributed computing architecture where every network node executes and records the same transactions, which are grouped into blocks. Only one block can be added at a time, and every block contains a mathematical proof that verifies that it follows in sequence from the previous block. In this way, the blockchain’s "distributed database" is kept in consensus across the whole network. Individual user interactions with the ledger (transactions) are secured by strong cryptography. Nodes that maintain and verify the network are incentivized by mathematically enforced economic incentives coded into the protocol.

In Bitcoin's case the distributed database is conceived of as a table of account balances, a ledger, and transactions are transfers of the bitcoin token to facilitate trustless finance between individuals. But as bitcoin began attracting greater attention from developers and technologists, novel projects began to use the bitcoin network for purposes other than transfers of value tokens. Many of these took the form of "alt coins" - separate blockchains with cryptocurrencies of their own which improved on the original bitcoin protocol to add new features or capabilities. In late 2013, Expanse's inventor Vitalik Buterin proposed that a single blockchain with the capability to be reprogrammed to perform any arbitrarily complex computation could subsume these many other projects.



================================================================================
Expanse Virtual Machine
================================================================================

Expanse is a programmable blockchain. Rather than give users a set of pre-defined operations (e.g. bitcoin transactions), Expanse allows users to create their own operations of any complexity they wish. In this way, it serves as a platform for many different types of decentralized blockchain applications, including but not limited to cryptocurrencies.

Expanse in the narrow sense refers to a suite of protocols that define a platform for decentralised applications. At the heart of it is the :ref:`Expanse Virtual Machine ("EVM") <the-EVM>`, which can execute code of arbitrary algorithmic complexity. In computer science terms, Expanse is "Turing complete". Developers can create applications that run on the EVM using friendly programming languages modelled on existing languages like JavaScript and Python.

Like any blockchain, Expanse also includes a peer-to-peer network protocol. The Expanse blockchain database is maintained and updated by many nodes connected to the network. Each and every node of the network runs the EVM and executes the same instructions. For this reason, Expanse is sometimes described evocatively as a "world computer".

This massive parallelisation of computing across the entire Expanse network is not done to make computation more efficient. In fact, this process makes computation on Expanse far slower and more expensive than on a traditional "computer". Rather, every Expanse node runs the EVM in order to maintain consensus across the blockchain. Decentralized consensus gives Expanse extreme levels of fault tolerance, ensures zero downtime, and makes data stored on the blockchain forever unchangeable and censorship-resistant.

The Expanse platform itself is featureless or value-agnostic. Similar to programming languages, it is up to entrepreneurs and developers to decide what it should be used for. However, it is clear that certain application types benefit more than others from Expanse's capabilities. Specifically, expanse is **suited for applications that automate direct interaction between peers or facilitate coordinated group action across a network**. For instance, applications for coordinating peer-to-peer marketplaces, or the automation of complex financial contracts. Bitcoin allows for individuals to exchange cash without involving any middlemen like financial institutions, banks, or governments. Expanse’s impact may be more far-reaching. In theory, financial interactions or exchanges of any complexity could be carried out automatically and reliably using code running on Expanse. Beyond financial applications, any environments where trust, security, and permanence are important – for instance, asset-registries, voting, governance, and the internet of things – could be massively impacted by the Expanse platform.

================================================================================
How does Expanse work?
================================================================================

Expanse incorporates many features and technologies that will be familiar to users of Bitcoin, while also introducing many modifications and innovations of its own.

Whereas the Bitcoin blockchain was purely a list of transactions, :ref:`Expanse's basic unit is the account <Accounts>`. The Expanse blockchain tracks the state of every account, and all state transitions on the Expanse blockchain are transfers of value and information between accounts. There are two types of accounts:

- Externally Owned Accounts (EOAs), which are controlled by private keys
- Contract Accounts, which are controlled by their contract code and can only be "activated" by an EOA

For most users, the basic difference between these is that human users control EOAs - because they can control the private keys which give control over an EOA. Contract accounts, on the other hand, are governed by their internal code. If they are "controlled" by a human user, it is because they are *programmed* to be controlled by an EOA with a certain address, which is in turn controlled by whoever holds the private keys that control that EOA. The popular term "smart contracts" refers to code in a Contract Account – programs that execute when a transaction is sent to that account. Users can create new contracts by deploying code to the blockchain.

Contract accounts only perform an operation when instructed to do so by an EOA. So it is not possible for a Contract account to be performing native operations like random number generation or API calls – it can do these things only if prompted by an EOA. This is because Expanse requires nodes to be able to agree on the outcome of computation, which requires a guarantee of strictly deterministic execution.

Like in Bitcoin, users must pay small transaction fees to the network. This protects the Expanse blockchain from frivolous or malicious computational tasks, like DDoS attacks or infinite loops. The sender of a transaction must pay for each step of the "program" they activated, including computation and memory storage.  These fees are paid in amounts of Expanse's native value-token, expanse.

These transaction fees are collected by the nodes that validate the network. These "miners" are nodes in the Expanse network that receive, propogate, verify, and execute transactions. The miners then group the transactions – which include many updates to the "state" of accounts in the Expanse blockchain – into what are called "blocks", and miners then compete with one another for *their* block to be the next one to be added to the blockchain. Miners are rewarded with expanse for each successful block they mine. This provides the economic incentive for people to dedicate hardware and electricity to the Expanse network.

Just as in the Bitcoin network, miners are tasked with solving a complex mathematical problem in order to successfully "mine" a block. This is known as a "Proof of Work". Any computational problem that requires orders of magnitude more resources to solve algorithmically than it takes to verify the solution is a good candidate for proof of work. In order to discourage centralisation due to the use of specialised hardware (e.g. ASICs), as has occurred in the Bitcoin network, Expanse chose a memory-hard computational problem. If the problem requires memory as well as CPU, the ideal hardware is in fact the general computer. This makes Expanse's Proof of Work ASIC-resistant, allowing a more decentralized distribution of security than blockchains whose mining is dominated by specialized hardware, like Bitcoin.


Learn about Expanse
==============================

[to be extended]


Blockchain and Expanse 101
----------------------------------

* `Explain bitcoin like I'm five <https://medium.com/@nik5ter/explain-bitcoin-like-im-five-73b4257ac833>`_ - an excellent introduction to blockchain technology and bitcoin to the mildly techsavvy layperson.

Infographics
--------------------------------
* coming soon


Comparison to alternatives
---------------------------------

* coming soon
