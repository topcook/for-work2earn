# For Work2Earn Project

This repository contains a sample project that you can use as the starting point
for your Ethereum project. It's also a great fit for learning the basics of
smart contract development.

## Quick start

The first things you need to do are cloning this repository and installing its
dependencies:

```sh
git clone https://github.com/topcook/for-work2earn.git
cd for-work2earn
npm install
```

Once installed, let's run Hardhat's testing network:

```sh
npx hardhat node
```

Then, on a new terminal, go to the repository's root folder and run this to
deploy your contract:

```sh
npx hardhat run scripts/deploy.js --network localhost
```

Finally, we can run the frontend with:

```sh
cd frontend
npm install
npm start
```

> Note: There's [an issue in `ganache-core`](https://github.com/trufflesuite/ganache-core/issues/650) that can make the `npm install` step fail. 
>
> If you see `npm ERR! code ENOLOCAL`, try running `npm ci` instead of `npm install`.

Open [http://localhost:3000/](http://localhost:3000/) to see your Dapp. You will
need to have [Metamask](https://metamask.io) installed and listening to
`localhost 8545`.

Set your network in MetaMask to 127.0.0.1:8545. You might also need to configure MetaMask to work well with Hardhat. To do that, go to Settings -> Networks -> localhost 8545 and change the Chain ID input to 31337 and 
symbol to TTFW.

What's happening here is that the frontend code to show the current wallet's balance is detecting that the balance is 0, so you wouldn't be able to try the transfer functionality.

By running: 

```sh
npx hardhat --network localhost faucet <your address>
```

## User Guide

In this project, we use hardhat network instead of other chains such as ethereum, bsc.
The owner address is 0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266 and the contract deploys the TTFW token.
The owner contract has 460 TTFW and the smart contract has 500 TTFW.
The 5 addresses are took part in this project because of test.
They are 
- 0x70997970C51812dc3A010C7d01b50e0d17dc79C8
  
  (private key: 0x59c6995e998f97a5a0044966f0945389dc9e86dae88c7a8412f4603b6b78690d, 10TTFW)
- 0x3C44CdDdB6a900fa2b585dd299e03d12FA4293BC
  
  (private key: 0x5de4111afa1a4b94908f83103eb1f1706367c2e68ca870fc3fb9a804cdab365a, 10TTFW)-
- 0x90F79bf6EB2c4f870365E785982E1f101E93b906
  
  (private key: 0x7c852118294e51e653712a81e05800f419141751be58f605c371e15141b007a6, 10TTFW)-
- 0x15d34AAf54267DB7D7c367839AAf71A00a2C6A65
  
  (private key: 0x47e179ec197488593b187f80a00eb0da91f1b9d0b13f8733639f19c30a34926a, 10TTFW)
- 0x9965507D1a55bcC2695C58ba16FB37d819B0A4dc
  
  (private key: 0x8b3a350cf5c34c9194ca85829a2df0ec3153be0318b5e2d3348e872092edffba, 0TTFW)

For testing, you should type this private key to your metamask wallet and can log in by using this wallet.
 
## What’s Included?

Your environment will have everything you need to build a Dapp powered by Hardhat and React.

- [Hardhat](https://hardhat.org/): An Ethereum development task runner and testing network.
- [Mocha](https://mochajs.org/): A JavaScript test runner.
- [Chai](https://www.chaijs.com/): A JavaScript assertion library.
- [ethers.js](https://docs.ethers.io/v5/): A JavaScript library for interacting with Ethereum.
- [Waffle](https://github.com/EthWorks/Waffle/): To have Ethereum-specific Chai assertions/mathers.
- [A sample frontend/Dapp](./frontend): A Dapp which uses [Create React App](https://github.com/facebook/create-react-app).


**Happy _building_!**
