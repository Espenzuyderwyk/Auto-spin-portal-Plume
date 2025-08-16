# Portal Plume Auto Spin Bot (Must Have min 2 PLUME) 
is a Node.js automation tool that calls the `startSpin()` function on the Plume `Spin` contract every fixed interval (default: **10 hours**), sending the specified PLUME amount automatically.

<img width="458" height="258" alt="GxPjrdXaIAMRM0Z" src="https://github.com/user-attachments/assets/7c2e69c0-6499-4472-8dd7-0fee4dc784d8" />

This bot is designed to:
- Run 24/7 on a server or locally.
- Keep track of the last successful spin to avoid duplicates.
- Retry failed spins with exponential backoff.
- Automatically manage gas fees or use fixed values.

## Features
- **Automatic execution**: Spins at a set interval (e.g., every 10 hours).
- **EIP-1559 support**: Uses `maxFeePerGas` and `maxPriorityFeePerGas`.
- **State persistence**: Remembers the last successful spin (`spin-state.json`).
- **Retry mechanism**: 2 min → 5 min → 10 min backoff on failure.
- **Balance check**: Ensures your wallet has enough PLUME for spin and gas.
- **Network validation**: Confirms you are connected to the correct Plume chain.

## Requirements
- **Node.js**: v18+ recommended
- **npm**: v8+ recommended
- A funded **Plume wallet** with PLUME for spins + gas fees
- RPC endpoint for Plume network (default: `https://rpc.plume.org`)

## Installation
Clone the project and install dependencies:

```bash
screen -S DailySpinPlume
```

```bash
git clone https://github.com/Espenzuyderwyk/Auto-spin-portal-Plume.git
```

```bash
cd Auto-spin-portal-Plume
```

```bash
npm install
```

## ⚙️ Environment Setup
Create a .env file in the root directory:

```bash
nano .env
```

Input your private key and wallet address

## ▶️ Run the Bot
Start

```bash
node autospin.js
```

## Disclaimer

This script is created for educational and personal experimentation purposes. It is not to be used for illegal activities, spam, or violations of GitHub rules.

- Be mindful of gas fees, slippage, and token volatility.
- This script is intended for testing and simulation purposes only.
- Use of this script is entirely the responsibility of the user.
- Do not use it to violate GitHub's Terms of Service.

#AutoSpinPlume #Plume #DailySpin #Web3
