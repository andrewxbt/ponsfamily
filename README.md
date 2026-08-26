# PONSFAMILY VOLUME MAKER ⚡

**A blazing-fast terminal trading bot for [pons](https://ponsfamily.com/) launches on Robinhood Chain — buy, sell, and generate volume on fresh token launches straight from your CLI, no browser required.**

Pons tokens launch straight into a live Uniswap V3 pool (no bonding curve), so every buy/sell is a real on-chain swap from the second a token goes live. ponsVolMaker talks to that pool directly — pool discovery, live pricing, and slippage-protected swaps — so you can act the moment a launch drops.

## Why it helps

- **Speed** — no UI to click through. Paste an address, confirm, done. Built for the first few seconds of a hot launch.
- **Built-in safety rails** — every buy/sell checks liquidity, balance, and slippage before it ever signs a transaction, so a bad launch or a moved price fails safely instead of burning your gas.
- **From a single buy to a whole trading desk** — one command for a quick buy, one mode for sustained volume, and a multi-wallet pool for spreading activity across several wallets at once.

## Features

- ⚡ **Buy / Sell** — instant swaps with live price, liquidity, and market cap shown before you confirm.
- 🔥 **Spam Buy Mode** — rapid-fire micro-buys at a set interval, with a live dashboard tracking every send.
- 🔁 **Volume Maker** — automated buy → hold → sell cycles to keep a chart active, with randomized timing so it doesn't look bots.
- 🔁👥 **Multi Vol Maker** — the same cycling, run concurrently across a whole pool of wallets, one atomic transaction per cycle.
- ⚡👥 **Multi Buy** — one buy from every wallet in your pool, fired in parallel.
- 💵 **Fund / Withdraw Wallets** — move ETH in and out of your wallet pool in one command.
- 💰 **Balance & Settings** — check holdings at a glance, tune default buy size / slippage / gas on the fly.
- 📡 **Launch listener** — a standalone watcher that flags new pons launches the moment they hit the chain.

## Quick start

```bash
npm install
cp .env.example .env
# add your PRIVATE_KEY to .env
npm start
```

Requires Node 18+.
