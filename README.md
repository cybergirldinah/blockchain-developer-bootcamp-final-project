#### Demo
[Demo](https://www.youtube.com/watch?v=TS497hNr8SY)  
[Gringotts Bank App](https://gringotts-defi.vercel.app/)

### Project Description
Wizards & witches can deposit their magical Ether currency into Gringotts bank for safe keeping. As a reward, Gringotts bank account hodlers will receive 1000 Galleons for making and hodling a deposit. Note that in the near future, before we launch our banking program to the main wizarding network on Ethereum, account hodlers must hodl a deposit for a minimum of 1 year without making any withdrawals to receive the Galleons reward. This will help Gringotts in its effort to create an ETH/GAL liquidity pool to further reward our account hodlers.

Here's how our system works:

#### Workflow

  1. User connects MetaMask wallet
  2. User deposits x ETH in their account
  3. User's balance is updated once transaction is mined
  4. User is rewarded Galleon tokens for using the protocol

## Project Structure

```
project
│   README.md
│   design_pattern_decisions.md
│   avoiding_common_attacks.md    
│   truffle-config.js
└───contracts
│   │   Galleon.sol
│   │   Gringotts.sol
│   │   Migrations.sol
└───migrations
│   │   1_initial_migration.js
│   │   2_deploy_contract.js
└───src
│   └───abis
│       │   Galleon.json
│       │   Gringotts.json
│   └───App.js
│   └───index.js
└───test
│       │   Gringotts.test.js

```

### Installation

#### Requirements

Please ensure `Truffle v5.4.12` is installed to be able to conduct tests. You will also need to start Ganache to connect to the local blockchain network. If the Gananche network ID is not 5777 please update the correct network ID in the truffle-config.js file on line 9.

#### Clone this repository

`git clone https://github.com/cybergirldinah/decentralized-banking-app`

#### Install Dependencies

Dependencies are stored in the `package.json` file. From the main project folder run:
`npm install`  

#### Set up truffle-config.js settings

Set the port to `7545` and networkID to `5777`:

```
development: {
     host: "127.0.0.1",     
     port: 7545,            
     network_id: "5777",       
    }
```

#### Truffle Test in Development Mode

In the main project folder run:
`truffle test`

#### Future Improvements

  1. Add price feed for ETH
  2. Allow users to earn more through Compound
  3. Create ETH/GAL liquidity pool on Uniswap
  
