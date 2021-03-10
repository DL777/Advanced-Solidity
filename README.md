# Advanced Solidity

In this project, I worked to create an ERC20 token that will be minted through a Crowdsale contract that I can leverage from the OpenZeppelin Solidity library.

This crowdsale contract will manage the entire process, allowing users to send ETH and get back PC (PupperCoin). This contract will mint the tokens automatically and distribute them to buyers in one transaction.

This contract inherits `Crowdsale`, `CappedCrowdsale`, `TimedCrowdsale`, `RefundableCrowdsale`, and `MintedCrowdsale` contracts.

I will conduct the crowdsale on Ropsten testnet in order to get a real-world pre-production test in.
