## Overview

This is a basic implementation of an ERC-20 token in Solidity, following the widely used Ethereum token standard. The contract supports common functionalities such as transferring tokens, approving third-party transfers, and querying balances.

## Features

- **Token Transfers:** Move tokens between accounts with the `transfer` function.
- **Third-Party Transfers:** Allow approved third parties to transfer tokens via `approve` and `transferFrom`.
- **Total Supply:** Define and mint the total supply at contract deployment.
- **Events:** `Transfer` and `Approval` events for monitoring token movements and approvals on the blockchain.

## Token Details

- **Name:** MyToken
- **Symbol:** MTK
- **Decimals:** 18
- **Initial Supply:** Set during deployment.

## How to Use

### Deployment

You can deploy this contract using tools like [Remix](https://remix.ethereum.org/) or via Truffle/Hardhat. 

To deploy:

1. In Remix, open the Solidity compiler, set the version to 0.8.x, and compile the contract.
2. Deploy the contract with an initial supply parameter.

```solidity
MyERC20Token myToken = new MyERC20Token(1000000);
