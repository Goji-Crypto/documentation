# Goji Labs Documentation

This repository holds the product documentation for Goji Labs. It is organized by product so that each line stands on its own and can evolve without entangling the others.

## Product areas

Goji Labs builds three distinct product areas:

1. **Goji Crypto** is the DeFi product family. It contains two product lines:
   - **Dynamic Liquidity (PL1 and PL2):** an AI managed synthetic index engine (PL1) and the index tokens it powers (PL2), including Hanu Yokia as the live proof of concept.
   - **Community Platform (PL3):** a staked curation and governance layer that lets a verified community decide which indices exist and funds those decisions through committed liquidity.
2. **Corralign** is an identity and LLM control model. It is a separate product and does not depend on the DeFi lines.
3. **Agent Orchestration** is a security first platform for governed, identity aware AI agent execution. It is also a separate product.

## Repository structure

```
documentation/
  README.md
  goji-crypto/
    dynamic-liquidity/      PL1 engine and PL2 index tokens
    community-platform/     PL3 curation and governance
  corralign/
  agent-orchestration/
  _archive/                 historical material, not maintained
```

Each folder carries its own README that states what the product is, the current document set, and what is planned.

## Document set status

| Product | Document | Status |
|---------|----------|--------|
| Dynamic Liquidity | 01 Concept Design | current |
| Dynamic Liquidity | 02 Detailed Design | planned |
| Dynamic Liquidity | 03 Technical Specification | planned |
| Dynamic Liquidity | 04 API Specification | planned |
| Community Platform | 01 Concept Design | current |
| Community Platform | 02 Detailed Design | planned |
| Corralign | Concept Design | imported |
| Agent Orchestration | Concept Design, v2 | imported |

## Migration from the old repository

The previous repository was a flat collection of PDFs. The table below maps each old item to its new home. Two early working documents are retired because the current Concept Design supersedes them.

| Old item | New location |
|----------|--------------|
| Goji Crypto Dynamic Liquidity.pdf | goji-crypto/dynamic-liquidity/research/original-whitepaper.pdf (archived reference) |
| AI-Driven Liquidity Management.pdf (VWAP) | goji-crypto/dynamic-liquidity/research/vwap-anchoring.pdf |
| stable_coins_notes.pdf | goji-crypto/dynamic-liquidity/research/stablecoin-notes.pdf |
| Part 1, AI-Powered Risk Assessment and Portfolio Optimization | goji-crypto/dynamic-liquidity/research/ai-risk-portfolio-optimization.pdf |
| Executive Briefing, AI-Driven DeFi Innovations | goji-crypto/dynamic-liquidity/research/ai-defi-innovations-briefing.pdf |
| AI-Driven liquidity Architecture.png | goji-crypto/dynamic-liquidity/assets/liquidity-architecture.png |
| VWAP zones.png | goji-crypto/dynamic-liquidity/assets/vwap-zones.png |
| lastest-update_02-06_2025.pdf | _archive/community-update-2025-02-06.pdf |
| ai/Corralign_LLM_Identity_Control_Model_v.012.pdf | corralign/concept-design.pdf |
| ai/AI Agent Orchestration - Concept Design.pdf | agent-orchestration/concept-design.pdf |
| ai/ai_agent_orchestration_v2.pdf | agent-orchestration/v2.pdf |
| ai/test | remove (stray file) |

New documents produced in the current design pass:

| New document | Home |
|--------------|------|
| Dynamic Liquidity Concept Design (v2) | goji-crypto/dynamic-liquidity/01-concept-design.md |
| Community Platform Concept Design (PL3) | goji-crypto/community-platform/01-concept-design.md |

Retired (delete from the new repo):

| Retired | Reason |
|---------|--------|
| Consolidated Reference (00) | folded into the v2 Concept Design |
| Concept Design v0.1 | superseded by the v2 Concept Design |

## Conventions

- Design documents are Markdown. Source papers and imported decks remain PDF until there is a reason to convert them.
- File names use lowercase kebab case with a leading number for ordered sets, for example `02-detailed-design.md`.
- Every document carries a version, a status, and an owner in its header.
- Prose uses standard US English and avoids dashes as punctuation. Sentences are written in full instead.
