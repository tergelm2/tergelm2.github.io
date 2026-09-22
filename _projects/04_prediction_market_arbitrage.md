---
name: Prediction-Market Arbitrage Tracker
tools: [Python, FastAPI, SSE, SQLite, Pytest]
image: /assets/projects/arb-trader.svg
description: A paper-trading system that matches equivalent markets, identifies pricing discrepancies, and tracks opportunities in real time.
---

<div class="case-study-hero">
  <p class="eyebrow">Independent project · Market data systems</p>
  <h1>Prediction-Market Arbitrage Tracker</h1>
  <p>A fault-aware pipeline for collecting prices, matching equivalent events, evaluating arbitrage, and monitoring paper trades.</p>
  <img src="{{ '/assets/projects/arb-trader.svg' | relative_url }}" alt="Prediction-market arbitrage system architecture">
</div>

## The system

Platform adapters normalize market data from Polymarket, Kalshi, and Manifold. A matcher groups equivalent events, an arbitrage engine evaluates multiple opportunity types, and a tracker records paper positions and outcomes. A FastAPI dashboard streams updates with server-sent events.

## Engineering choices

- Paper trading is the default and live submission is intentionally gated.
- The supervisor coordinates subsystem shutdown and restarts the dashboard with bounded backoff.
- Tests cover matching, opportunity evaluation, execution safeguards, and tracking.
- SQLite keeps development and demonstrations reproducible.

## Current status

This project is portfolio-ready as an engineering case study. Before a public repository is linked, I plan to add a recorded demonstration and a clearly documented data-source policy.
