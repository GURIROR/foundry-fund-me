# Foundry Fund Me

A decentralized fundraising smart contract built using Foundry, Solidity, and Chainlink Oracles.

## Overview

Foundry Fund Me enables decentralized fundraising on Ethereum-compatible networks, leveraging Chainlink price feeds to ensure secure and accurate ETH/USD conversions. Users can seamlessly contribute ETH towards fundraising goals, with minimum funding amounts dynamically calculated in USD.

## Features

- Decentralized Fundraising: Allow users to contribute ETH securely and transparently.
- Chainlink Integration: Accurate real-time ETH/USD pricing via Chainlink Data Feeds.
- Automated Minimum Contribution: Dynamically calculated contributions based on the latest ETH/USD rate.
- Secure Withdrawals: Only the owner can withdraw the collected funds securely.
- Gas Optimization: Optimized smart contracts for efficient deployment and reduced transaction costs.

## Tech Stack

- Solidity
- Foundry (Forge & Anvil)
- Chainlink Oracles
- Ethereum (or compatible testnets/mainnets)

## Installation

### Clone the Repository
```bash
git clone https://github.com/GURIROR/foundry-fund-me.git
cd foundry-fund-me
```

### Install Dependencies
Make sure you have Foundry installed. If not, [follow the Foundry installation guide](https://github.com/foundry-rs/foundry).

```bash
forge install
```

## Compile Smart Contracts

```bash
forge build
```

## Run Tests

```bash
forge test
```

## Deploying Contracts

Set up your environment variables in `.env` file:

```env
PRIVATE_KEY=your_private_key
RPC_URL=your_rpc_url
ETHERSCAN_API_KEY=your_etherscan_api_key
```

Deploy using the provided Forge script:

```bash
forge script script/DeployFundMe.s.sol --rpc-url $RPC_URL --broadcast --verify -vvvv
```

## Usage

- Users can send ETH to the deployed smart contract address to fund.
- Only the owner (deployer) can withdraw accumulated funds.

## Contributing

Feel free to open issues, submit pull requests, or provide suggestions to enhance the functionality of the smart contract.

## License

This project is open-sourced under the MIT License. See [LICENSE](LICENSE) for details.

