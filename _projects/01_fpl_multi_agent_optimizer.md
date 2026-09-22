---
name: FPL Multi-Agent Optimizer
tools: [Python, LangGraph, XGBoost, FastAPI, React]
image: /assets/projects/fpl-agent.svg
description: A team-built decision system that combines ML forecasts with specialized agents for lineup, transfer, and captaincy strategy.
---

<div class="case-study-hero">
  <p class="eyebrow">Team project · AI engineering</p>
  <h1>Fantasy Premier League Multi-Agent Optimizer</h1>
  <p>A product-oriented agent system that turns historical football data and model predictions into explainable gameweek decisions.</p>
  <img src="{{ '/assets/projects/fpl-agent.svg' | relative_url }}" alt="FPL multi-agent system diagram">
</div>

## The problem

Fantasy Premier League decisions combine noisy forecasts, hard squad constraints, risk tolerance, and a constantly changing fixture calendar. A single prediction score is not enough—the system also needs to explain how that score should affect transfers, lineup selection, captaincy, and chip usage.

## The system

The project combines an XGBoost forecasting pipeline with specialized LangGraph agents. A FastAPI backend exposes predictions and agent recommendations to a React interface.

<div class="case-study-grid">
  <div class="case-study-stat"><strong>3 specialized agents</strong><span>Statistician, Sporting Director, and Manager</span></div>
  <div class="case-study-stat"><strong>Walk-forward evaluation</strong><span>Gameweek-aware validation instead of random splitting</span></div>
  <div class="case-study-stat"><strong>Full product stack</strong><span>Model pipeline, agent API, and interactive frontend</span></div>
</div>

## My contribution

I developed the Manager Agent specification and a standalone prototype of its decision flow. The agent evaluates every valid formation, selects a risk-adjusted starting XI, orders the bench, chooses captain and vice-captain candidates, recommends chips, and produces a human-readable explanation. Its decisions are deterministic and testable.

## What I learned

- Separate prediction from decision policy so each layer can be tested independently.
- Encode domain constraints directly into agent state and validation steps.
- Make explanations a first-class output, not an afterthought.

<div class="portfolio-actions">
  <a class="portfolio-button portfolio-button-primary" href="https://github.com/moyez48/fpl-optimizers-agentic-ai" target="_blank" rel="noopener">Team repository ↗</a>
</div>
