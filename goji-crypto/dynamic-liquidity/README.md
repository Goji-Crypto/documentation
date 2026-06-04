# Dynamic Liquidity (PL1 and PL2)

An AI managed synthetic index engine and the index tokens it powers.

## What it is

Hanu is a dynamically managed, onchain synthetic index. Its market price is the depth weighted blend of its live trading pairs. An AI policy rotates that blend between risk constituents and a defensive USDC sleeve based on signals across several timeframes. The objective is drawdown reduction and volatility management relative to a static hold of the same constituents. It is not a price stability or appreciation guarantee.

Two hard invariants define the engine:

1. Hanu is never sold into a pool. Rotations touch only the counter asset legs.
2. The operator never buys or sells Hanu to move its price. Price is set by external arbitrage; the operator influences it only by where it places depth.

## Documents

- `01-concept-design.md`: current. Defines the mechanism, the honest performance character (the exit drives drawdown reduction, the re entry is where the edge lives), the conceptual architecture, the operating modes from data collection to guarded autonomy, and the signal and policy design.
- `02-detailed-design.md`: planned. Takes each subsystem and open question down to concrete specifications.
- `03-technical-spec.md`: planned.
- `04-api-spec.md`: planned.

## Supporting material

- `research/`: the prior papers and notes (VWAP anchoring, stablecoin notes, the DeFi innovations series, the archived original whitepaper).
- `assets/`: architecture and VWAP diagrams.

## Before the Detailed Design

A backtest harness that runs the trend confirmation policy on real constituent data and reports drawdown, return, and whipsaw should come first. It tells you whether the turn timing edge that the whole strategy rests on actually exists at realistic transaction cost.
