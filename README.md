# JAM Research

This repository is primarily focused on researching JAM and associated technologies. It will host research notes, code snippets, and various resources pertinent to JAM.

The primary objective is to assist the Subscan team in comprehending the JAM architecture and its advantages, while exploring the potential to develop a JAM-friendly explorer.

## Overview

Back in 2022, we could catch a glimpse of the early form of JAM in the shadow of Polkadot.

> [Polkadot v1.0: Sharding and Economic Security](https://polkadot.com/blog/polkadot-v1-0-sharding-and-economic-security#approval-checking-and-finality)
>
> In fact, our base unit of parachain consensus isn't actually a parachain, but something that we call an availability core or core for short. These are something like CPU cores: they operate in parallel, and have work scheduled onto them in discrete time-slots. Each parachain has its own dedicated core, which means that it's always scheduled onto a particular core. However, we can also multiplex multiple chains onto a single core. The only difference is the scheduling algorithm.

Now, let’s highlight some important points that we should keep in mind initially.

> [What is the difference between Optimistic Rollups and ZK-Rollups?](https://www.coinbase.com/en-sg/learn/tips-and-tutorials/what-is-the-difference-between-optimistic-rollups-and-zk-rollups)
>
> Rollups are Layer 2 scaling solutions that process transactions off-chain and then bundle the transaction data into batches to submit them on the corresponding Layer 1 blockchain. This reduces congestion and computation load on the main blockchain, thereby increasing transaction throughput. The two main types of rollups are Optimistic Rollups and Zero-Knowledge Rollups.

> [Layer Two and Rollups](https://wiki.polkadot.network/docs/learn-comparisons-rollups)
>
> Whereas rollups are considered solutions for L2 protocols, Polkadot include this functionality natively through its Parachains Protocol. The Parachains Protocol, which is how Polkadot handles network's sharding is meant to accomplish the combined goals of providing security, scalability, and availability.

> [The Path of a Parachain Block](https://polkadot.com/blog/the-path-of-a-parachain-block)
>
> Now is an apt time to make a key distinction: Polkadot does not guarantee a valid state; it guarantees a valid state transition. Polkadot validators do not inspect every value in a parachain’s state, only those that are modified, where it ensures that the modification is valid. If a chain joins the Polkadot network with a valid state and executes all of its transitions under the umbrella of Polkadot security, then it will have a valid state.

> [Polkadot's JAM Chain](https://wiki.polkadot.network/docs/learn-jam-chain)
>
> SAFROLE is a block production algorithm, a simplification of SASSAFRAS. It excludes some components that may be useful for parachains. So parachains may probably stick with SASSAFRAS rather SAFROLE.

## Thinking

### JAM Explorer

There can be an expolrer for JAM, but what will it look like? What will be the main features of the explorer? There isn't transactions exist in JAM, so who will be the users of the explorer?

### JAM's Service Explorer

JAM likens itself to a supercomputer, with validators at its core, and the L2 or various applications as the services within the computer. Following this line of thought, do these services require a monitor?

## Material

### Paper

#### Beginner

-   [Polkadot JAM Explained. Simply!](https://polkadotters.medium.com/polkadot-jam-explained-simply-825ec8b24607)
-   [What is JAM? Polkadot's Biggest Ever Upgrade Explained](https://decrypt.co/resources/what-is-jam-polkadots-biggest-ever-upgrade-explained)

#### Intermediate

-   [Polkadot v1.0: Sharding and Economic Security](https://polkadot.com/blog/polkadot-v1-0-sharding-and-economic-security)
-   [Polkadot's JAM Chain](https://wiki.polkadot.network/docs/learn-jam-chain)
-   [Demystifying JAM](https://blog.kianenigma.nl/posts/tech/demystifying-jam)
    -   [zh-CN](material/demystifying-jam-zh-CN.md)

#### Advanced

-   [JAM Gray Paper](https://graypaper.com)
-   [Efficient Execution Auditing for Blockchains under Byzantine Assumptions](https://eprint.iacr.org/2024/961)
-   [Announcing PolkaVM - a new RISC-V based VM for smart contracts (and possibly more!)](https://forum.polkadot.network/t/announcing-polkavm-a-new-risc-v-based-vm-for-smart-contracts-and-possibly-more/3811)
-   [JAM Simple Networking Protocol (JAMNP-S)](https://hackmd.io/@polkadot/jamsnp)
-   [SASSAFRAS](https://research.web3.foundation/Polkadot/protocols/block-production/SASSAFRAS)

### Video

-   [Gavin Wood: The Gray Paper Interview - JAM & the Future of Polkadot - Behind the Code: Web3 Thinkers](https://www.youtube.com/watch?v=O3kRAVBTkfs)
-   [JAM Gray Paper - Gavin Wood Lecture Series](https://www.youtube.com/watch?v=wbnTnBQNDr4&list=PLwcnAOKMj-Ab7sDej2P4peqGxu2mTGYNy)

### Code

-   [jamtestvectors](https://github.com/w3f/jamtestvectors)

### Tool

-   [pvm-debugger](https://github.com/FluffyLabs/pvm-debugger)

### Other

-   [Decentralized JAM](https://jam.web3.foundation)
