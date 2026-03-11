# Shelby Testnet Guide: Faucet & Upload Image to ShelbyNet

A beginner-friendly guide and TypeScript example to participate in the **Shelby Protocol** testnet (built on Aptos).

Shelby is a decentralized hot blob storage protocol optimized for AI, streaming, and read-heavy workloads.  
Testnet name: **shelbynet**  
Official docs: https://docs.shelby.xyz  
TypeScript SDK: https://docs.shelby.xyz/sdks/typescript  
Explorer: https://explorer.shelby.xyz/shelbynet

## Goals of this repo
- Claim test tokens (APT + ShelbyUSD) from faucet
- Upload an image (or any file) to ShelbyNet using TypeScript SDK
- Simple Node.js script to get you started

## Prerequisites
- Node.js ≥ 18
- Yarn or npm
- Petra Wallet (Aptos wallet) → https://petra.app
- Join Shelby Discord for updates: https://discord.com/invite/shelbyserves (recommended)

## Step 1: Setup Petra Wallet for Shelby Testnet (shelbynet)
1. Install Petra Wallet browser extension
2. Create or import wallet
3. Switch network to **Shelbynet**  
   → See guide: https://docs.shelby.xyz/tools/wallets/petra-setup
4. Copy your wallet address (starts with `0x...`)

## Step 2: Claim Test Tokens from Faucet
Shelby testnet requires:
- APT (for gas fees)
- ShelbyUSD (for storage operations like upload)

### Option A: Via CLI (recommended for developers)
```bash
# Install Shelby CLI globally
npm install -g @shelby-protocol/cli

# See faucet URL for your active account
shelby faucet --network testnet --no-open
# → Outputs: https://faucet.shelbynet.shelby.xyz?address=YOUR_ADDRESS

# Open the link in browser → claim tokens
