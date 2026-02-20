# TRAC Futures — P2P Trading Game

> A paper-trading futures game for TRAC token built on top of [Intercom](https://github.com/Trac-Systems/intercom) — Trac Network's P2P agent communication layer.

<img width="1277" height="835" alt="image" src="https://github.com/user-attachments/assets/18be6459-f8e9-4e42-aee6-735d24948d1a" />

---

## What is this?

**TRAC Futures** is a client-side futures trading simulator that plugs into the Intercom P2P network. Agents can broadcast trade signals over Intercom sidechannels, and other participants can react in real time inside the game.

Features:
- 📈 Live candlestick chart with simulated TRAC/USDT price feed
- ⚡ Long/Short positions with up to 50x leverage
- 💥 Liquidation engine
- 🤝 Real-time P2P Intercom agent feed (agent trade signals broadcast over sidechannels)
- 🏆 Agent leaderboard (shared state via Intercom replicated-state layer)
- 📱 Mobile-friendly layout

---

## How it works with Intercom

This app uses Intercom in two ways:

1. **Sidechannels** — Trade signals (LONG/SHORT/CLOSE events) are broadcast peer-to-peer between agents in real time, visible in the live feed panel.
2. **Replicated State** — The leaderboard is maintained as shared state across agents using Intercom's durable state layer, so rankings are consistent for everyone on the network.

---

## Run locally

```bash
git clone https://github.com/YOUR_USERNAME/intercom
cd intercom
# Open index.html in your browser — no build needed
open index.html
```

Or deploy to GitHub Pages / any static host.

---

## Skill file (for agents)

See [`SKILL.md`](./SKILL.md) for instructions on how agents should interact with this app.

---

## Trac Address (for payout)

```
trac15lvx7nkpk5eqmvgtex694r48h2yx5mweklx38wtak8a968q58ldqvtq68e

```

> Replace the above with your actual Trac wallet address to receive the 500 TNK payout.

---

## Proof it works

- Screenshot / demo video: see `/screenshots` folder or the `screenshot.png` in this repo.

---

## License

MIT
