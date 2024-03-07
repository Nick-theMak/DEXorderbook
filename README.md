# DEX Orderbook

Welcome to the Decentralised Orderbook Exchange. This project demonstrates a deployed decentralised exchange with swap, deposit, and withdrawal functionality as well as a dashboard for displaying open orders and trades, simulating a completely functional crypto trading dashboard.

## Technology Stack & Tools

- Solidity (Writing Smart Contracts & Tests)
- Javascript (React & Testing)
- [Hardhat](https://hardhat.org/) (Development Framework)
- [Ethers.js](https://docs.ethers.org/v5/) (Blockchain Interaction)
- [React.js](https://react.dev/) (Frontend Framework)




## Requirements For Initial Setup

- Install [NodeJS](https://nodejs.org/en/)
- - Have [MetaMask](https://metamask.io/) Web Extension installed and configured for a [Hardhat Network](https://docs.metamask.io/wallet/how-to/run-devnet/) (Note: in the `config.js` file you will see the specified chainId to configure the wallet)

## Setting up the Environment

### 1. Clone/Download the Repository

### 2. Open terminal in the project's root directory

### 3. Install Dependencies:
```
$ npm install
```
    
### 4. Run tests
```
$ npx hardhet test
```

See the list of tests for each smart contract:
  1. Token.js
  2. Exchange.js
     
Note: tests involving a third smart contract for 'Aggregator.sol' where the aggregator logic exists on a smart contract level are not being used in the application due to unesscecary gas fees, making the Decentralised application less efficient.

The tests for the third contract still remain as a 'proof of concept' that the same logic can be implemented on a smart contract level.

### 5. Start Hardhat node

```
$ npx hardhat node
```

### 6. Run Deployment and Seed Script

Deploys the smart contracts to the local hardhat node
```
$ npx hardhat run scripts/1_deploy.js --network localhost
```

Fill the exchange with data to visualise Dapp functionality
```
$ npx hardhat run scripts/2_seed-exchange.js --network localhost
```

### 7. Start frontend
```
$ npm run start
```

