## how to build on linea with hardhat (draft)
(testnet and mainnet)
-----------------------------
--introduction
---setting up your enviroment
---importing linea to metamask
---setting up ypur hardhat enviroment for linea
--deploying on linea
--verifying your contract
------------------------------------
Linea is a zerro knowledge rollup chains


## Objective

By the end of this tutorial you should be able to write a contract and deploy it with create2 on the CELO blockchain.

## Prerequisites

- Understanding of [Solidity](https://soliditylang.org/): It is important to have a strong understanding of Solidity as it is the main programming language for creating smart contracts on the Celo blockchain.

- Command line proficiency: Basic familiarity with using command line tools such as the terminal or Command Prompt is necessary for running commands and scripts.

- Proficiency in [Hardhat](https://hardhat.org/): It is essential to have a good grasp of using Hardhat, a development environment designed for writing, testing, and deploying smart contracts on the Celo blockchain.

## Requirements

- A text editor: For this tutorial, we will make use of [Visual Studio Code](https://code.visualstudio.com/).
- You will need to have [Node.js](https://nodejs.org/en) installed on your system, with version V10. or higher.
- Node Package Manager [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) used for installing and managing dependencies.
-  Install [MetaMask Wallet](https://metamask.io/download/).

## A brief intro to Linea
Linea is a fully EVM equivalent zero-knowledge rollup (zk-rollup), designed to scale Ethereum with higher throughput and lowered transaction fees.
An EVM-equivalent network, scaling the Ethereum experience. Secured with a zero-knowledge rollup to Ethereum, built on quantum-resistant, lattice-based cryptography, powered by Consensys.

Linea relies on an innovative, internally-built, lattice-powered prover which utilizes zkSNARK technology. It enables proofs to be generated quickly and yet does not require a trusted setup, which has long been a flaw of zkSNARK technology.

To read more on [zkevm](https://consensys.net/zkevm/) 


### Benefits of Using Linea

1. **Low gas fees:**  Build dApps that users can interact with at scale.

2. **EVM equivalent:** Fully compatible with existing tooling, infrastructure, IDEs and wallets.

3. **Secured by Ethereum:** Backed by the security of Ethereum, where all rollup transactions are verified on-chain by a decentralized community of over 500k validators.

4. **Next gen scalability:** Innovative lattice-based zkSNARK prover generates fast zero-knowledge proofs.

5. **Developer-friendly design:** Built to minimize onboarding time, the rollup abstracts away ZK complexity, uses ETH for gas and has no reliance on third party transpilers or bespoke middleware

















# Usage
1. Install the [MetamaskWallet](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn) from the google chrome store.
2. Create a wallet.
3. Go to [https://www.infura.io/faucet/linea](https://www.infura.io/faucet/linea) 
and get tokens for the Linea Goerli.
4. Switch to the Linea Goerli in the MetamaskWallet.



This section should walk you through everything you need to get started:

Set up your wallet   
Linea comes with metamask directly so you don;t need to impoort or configure your metamask
Get funds from a faucet

here: [https://www.infura.io/faucet/linea]
here: [https://www.covalenthq.com/platform/faucet/]
here: [https://linea.faucetme.pro/]

you can also bridge your goerli eth to linea 
here[https://bridge.linea.build/]
Connect your wallet in the top-right corner of the page.

Verify that the bridge is set to Ethereum → Linea Mainnet, and that manual claiming is enabled.

Enter the amount of ETH you want to bridge over to Linea Mainnet, and select the Start Bridging button.
nb: check that your network is on tetsnet if you are bridging your testnet token.

Bridge some funds
Deploy your first contract
If you run into a problem, step on over to the Linea Support page and let us know.


 >**_Note_**: check that your network is on tetsnet if you are bridging your testnet token.

setting up hardaht
open terminal
bash
```
mkdir linea-tutorial
```
cd linea-tutorial

npm init
npm install --save-dev hardhat
npx hardhat