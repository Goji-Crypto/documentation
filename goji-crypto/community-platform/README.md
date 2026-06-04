# Community Platform (PL3)

A staked curation and governance layer for the Goji Crypto index family.

## What it is

Participants complete KYC, then stake USDC to propose and back suggestions about which sector indices exist and how they are parameterized. Vote weight is quadratic in the amount staked, so influence grows far slower than capital. Backing for winning proposals converts into transparent, claim bearing liquidity that launches the index it curated. The platform sets the policy envelope; the Dynamic Liquidity engine executes within it.

This is a token curated registry with liquidity bootstrapping, not a DAO.

## The mechanism in three legs

The design rests on three controls that each close the next one's weakness:

1. USDC staking gives Sybil resistance and funds the result.
2. Quadratic voting keeps capital from becoming control.
3. KYC removes the multi wallet attack on quadratic voting and creates the audit trail.

## Non negotiable guardrails

These sit below governance and no vote can change them:

- No pooled capital may execute discretionary buys that support the price of any Goji token.
- Vote weight is always the square root of stake.
- Contributed capital that becomes liquidity always carries a disclosed claim.

## Documents

- `01-concept-design.md`: current.
- `02-detailed-design.md`: planned. Blocked on the legal questions in the Concept Design reaching counsel first.

## Open business question

A B2B model is under exploration in which ETF firms and smaller asset managers run their own index products on Goji workflow and scaffolding. This is being studied separately because it changes the legal posture: as an infrastructure provider, Goji is lighter on regulatory burden and the client manager carries the fund obligations.
