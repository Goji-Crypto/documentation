# Goji Crypto

The Goji Crypto DeFi product family. It contains two product lines that depend on each other in one direction: the Community Platform governs index products that the Dynamic Liquidity engine runs.

## Product lines

- **Dynamic Liquidity** (`dynamic-liquidity/`) is the core. It is the AI managed synthetic index engine (PL1) and the index tokens it powers (PL2). Everything else in this family rests on it, so it is the line to finish first.
- **Community Platform** (`community-platform/`) is the curation and governance layer (PL3). It lets a verified community propose, vote on, and fund index products through staked liquidity. It sets parameters; it does not execute trades.

## Existing tokens

The four tokens already created (Hanu Yokia, Mia Neko, Goji, Safaia Gabanansu) are separate from the platform mechanics. Hanu serves as the live proof of concept index and, in the Community Platform, as the tipping currency. The roles of the other three in the managed index set are an open question in the Dynamic Liquidity Concept Design.

## Legal posture

A family of actively managed pooled baskets, and a platform that pools committed capital, sits close to regulated fund and securities activity. Each Concept Design carries an explicit set of legal questions that must reach counsel before its Detailed Design is built.
