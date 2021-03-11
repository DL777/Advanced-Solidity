# Advanced Solidity

In this project, I worked to create an ERC20 token that will be minted through a Crowdsale contract that I can leverage from the OpenZeppelin Solidity library.

This crowdsale contract will manage the entire process, allowing users to send ETH and get back PUP (PupperCoin). This contract will mint the tokens automatically and distribute them to buyers in one transaction.

This contract inherits `Crowdsale`, `CappedCrowdsale`, `TimedCrowdsale`, `RefundableCrowdsale`, and `MintedCrowdsale` contracts.

I will conduct the crowdsale on Ropsten testnet in order to get a real-world pre-production test in.

# PupperCoin.sol

 I start by creating in Remix a standard `ERC20Mintable` token in contract ` PupperCoin.sol`. The code for this coing is attached in file `PuppeCoin` and is as follows:

![PupperCoinCode](Screenshots/PupperCoinCode.png)

# PupperCoinSale.sol

Next I create `PupperCoinSale.sol` which inherits `PupperCoin.sol` as well as `Crowdsale.sol`, `MintedCrowdsale.sol`,  `CappedCrowdsale.sol`, `TimedCrowdsale.sol` and `RefundablePostDeliveryCrowdsale.sol`.

The code for `PupperCoinSale.sol` is shown here:

![PupperCoinCode](Screenshots/pcsale.png)

# PupperCoinSaleDeployer.sol

This contract deploys crowdsale and its code is shown here:

![deploy](Screenshots/deploy.png)
