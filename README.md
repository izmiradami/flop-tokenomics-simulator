# FLOP Tokenomics Simulator

An interactive, single-file web tool that visualizes the tokenomics of the **Flop Network** — a proof-of-useful-inference blockchain where GPU owners earn `$FLOP` for verified AI inference.

**Live demo:** _enable GitHub Pages to get a link (see below)_

## What it does

- **Supply simulator** — Adjust block reward, block time, halving period/count, and horizon with sliders and watch the cumulative supply curve redraw live, with halving markers and a hover readout.
- **Allocation donut** — Interactive breakdown of the year‑10 supply split across miners, airdrop, team + foundation, validators, brokers/agents, and staking.
- **Genesis airdrop breakdown** and full **network parameters** + roadmap.
- **4‑layer verification** explainer (TEE, TOPLOC, re‑execution, stake & slashing).

The emission model is computed from the whitepaper's own logic — `block reward × (86,400 / block time) × halving period`, halving each period, plus the 3.5B genesis pre‑mint — and reproduces the whitepaper's ~17.2B year‑10 supply target.

## Tech

- 100% client‑side. One `index.html` file, no build step, no backend, no dependencies (Google Fonts only).
- Light/dark theme aware.
- Accessible, colorblind‑safe chart palette.

## Run locally

Just open `index.html` in any browser.

## Publish with GitHub Pages

1. Push this repo to GitHub.
2. Repo **Settings → Pages**.
3. Under **Build and deployment**, set **Source: Deploy from a branch**, branch **main**, folder **/ (root)**, and Save.
4. After a minute your live URL appears at the top of the Pages settings — that is your shareable demo link.

## Disclaimer

This tool visualizes provisional figures from the Flop Network draft whitepaper (v0.1). Numbers may change; the definitive spec is the (not yet final) Yellow Paper. Not investment advice.
