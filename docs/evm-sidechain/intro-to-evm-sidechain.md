---
html: intro-to-evm-sidechain.html
parent: xrpl-interoperability.html
blurb: Introduction to the EVM compatible XRP Ledger Sidechain
labels:
  - Interoperability
status: not_enabled
---
# Introduction to EVM Compatible XRP Ledger Sidechain

<embed src="/snippets/_evm-sidechain-disclaimer.md" />

The Ethereum Virtual Machine (EVM) compatible XRP Ledger sidechain is a fast and secure blockchain that brings web3 applications to the XRP Ledger community.

- Explorer: [https://evm-sidechain.xrpl.org](https://evm-sidechain.xrpl.org)
- Public RPC: [https://rpc-evm-sidechain.xrpl.org](https://rpc-evm-sidechain.xrpl.org)
- Bridge UI: [https://bridge.devnet.xrpl.org]( https://bridge.devnet.xrpl.org/)

Some highlights of the EVM sidechain include:

- Support for 1000 transactions per second, enabling large loads and throughput.
- Low transaction confirmation times, producing a block every 5 seconds.
- 1 block finalization time; once a block is added to the chain and confirmed, it's considered final.
- Full Ethereum Virtual Machine (EVM) compatibility, enabling you to connect your wallet and interact with or deploy smart contracts written in Solidity. <!-- STYLE_OVERRIDE: wallet -->


## Consensus

The EVM sidechain runs on a proof of authority (PoA) consensus algorithm. Proof of authority gives a designated number of blockchain actors the power to:

- Validate transactions or interactions on the network.
- Update the network's registry.

One or more validating machines on the network are then responsible for generating new blocks of transactions to include on the blockchain.

The underlying technology for the XRPL sidechain consensus is CometBFT, a fork of [Tendermint](https://tendermint.com/), which is a Byzantine fault tolerant engine for building blockchains.

The blockchain uses the `cosmos-sdk` library on top of CometBFT to create and customize the blockchain using its built-in modules. The EVM sidechain uses the [Ethermint](https://github.com/evmos/ethermint) `cosmos-sdk` module to provides EVM compatibility.

If you are interested in running your own node, please see: [Join the XRP Ledger EVM Sidechain Devnet](join-evm-sidechain-devnet.md).

## Interoperability Using the EVM Sidechain

The EVM sidechain is directly connected to XRP Ledger through the XRPL bridge [https://bridge.devnet.xrpl](https://bridge.devnet.xrpl.org/). Through this bridge, you can connect to the EVM Sidechain and use its features.

## See Also

[Get Started with EVM Sidechain](get-started-evm-sidechain.md)
