# Manifest — USDC Payment Tracker (Built on Arc Testnet)

A lightweight web dashboard for tracking USDC payment status in real time on **Arc Testnet**. Built for the export/SME vendor use case: instead of waiting 1–3 days for manual bank wire confirmation, invoice status here updates automatically the moment USDC is received on-chain.

## Features
- Connect wallet (MetaMask) with automatic Arc Testnet network setup
- View native USDC (gas) balance and ERC-20 USDC balance
- Create invoices and track their status (Pending → Paid)
- Incoming USDC transaction history, read directly from on-chain `Transfer` events

## Getting started
No build step required — just open `manifest-en.html` directly in a browser, or run it with Live Server (VS Code).

1. Clone this repo
2. Open `manifest-en.html` with Live Server
3. Click **Connect Wallet** and approve adding the Arc Testnet network in MetaMask
4. Get testnet USDC from the [Circle faucet](https://faucet.circle.com) (select Arc Testnet)

## Network configuration
| Item | Value |
|---|---|
| Chain ID | `5042002` |
| RPC URL | `https://rpc.testnet.arc.network` |
| Explorer | `https://testnet.arcscan.app` |
| USDC (ERC-20) | `0x3600000000000000000000000000000000000000` |

## Notes
- Payment detection is based on total wallet balance change, not precise per-invoice matching — suitable for demos/hackathons.
- This project is built on Arc Network and is not officially affiliated with Circle/Arc.

## License
MIT
