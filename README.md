# Ethereum Coin Flipper
## Introduction
Ethereum coin flipper is a decentralized app that enables 2 participants to perform a winner-takes-all pseudo-random coin flip. This is how it works:
1. A new instance of a coin flip contract is created
2. A participant (player 1) deposits a certain amount of ethereum to the contract
3. A second participant (player 2) can then accept the terms of the contract by depositing the same amount of ethereum to the contract
4. The virtual coin is flipped and the amount of ethereum in the smart contract is deposited to either player 1 or player 2 depending on the outcome.
## Demo
Currently, a demo is live on the Ropsten Test Net [here](http://185.224.91.89/). Use MetaMask or Mist to execute the transactions.
## Installaion
1. Install Truffle globally
```
$ npm i -g truffle
```
2. Clone repository
```
$ git clone https://github.com/HarmvZ/eth-coin-flipper.git
```
3. Go in project folder and fetch dependencies
```
$ cd eth-coin-flipper
$ npm i
```
4. Run Truffle development console
```
$ truffle develop
```
5. Compile and migrate contracts
```
> compile
> migrate

```
6. Start development server (run this in a new shell)
```
$ npm run start
```
7. Now you can use your browser and MetaMask to start flipping coins on http://localhost:3000
## Improvements
* Fix Material Design Lite number input
* Streamline contract interaction by combining transactions: CoinflipCollection.addNew() + Coinflip.makeWager() and Coinflip.acceptWager() + Coinflip.resolveBet()
* Add players
* Improve randomness
* Add minimum wager amount
## Why?!
I created this app to learn more about developing on the Ethereum VM.
## Credits
This project is created with the [official Truffle React box](http://truffleframework.com/boxes/react). 
The coin flip smart contract is based on [this example](https://gist.github.com/AlwaysBCoding/fa141a313f404b585016ff2a1e62adaf) by Decipher Media.
## Donate
BTC 16eBpKYVTHyg1XdVJ1gNGGK3wrpcGWSGne
ETH 0xfAA23b0173eD6A34aa4B880fA3aC8dAE71fdE6F9