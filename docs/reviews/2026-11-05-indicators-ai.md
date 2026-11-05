# GitHub sweep: AI trading with technical indicators — 2026-11-05

This targeted sweep looked for resources that use LLMs or reinforcement learning to trade with technical indicators and chart patterns, with no date restriction. Over 50 GitHub repository searches covered indicator-based RL, LLM and vision agents reading indicators or candlestick charts, Pine Script and TradingView agents, and indicator libraries used for feature engineering. A literature search for papers with official code followed. Entries were screened against [CONTRIBUTING.md](../../CONTRIBUTING.md). Descriptions follow each project's README or documentation. This is documentation review, not reproduction.

## Added

| Section | Entry | Basis |
| --- | --- | --- |
| Trend Following | TA-Lib (Python wrapper) | Reference indicator and pattern library; BSD; very widely used |
| Trend Following | ta | Pure-Python indicator library aimed at feature engineering; MIT |
| ML and AI Strategies | FreqAI | Adaptive ML and RL (stable-baselines3) on indicator features inside Freqtrade; JOSS 2022; GPL-3.0 |
| LLM-Based Trading Agents | QuantAgent | Indicator, chart-pattern (vision), trend, and risk agents; arXiv 2509.09995; official code, MIT |
| Research Papers: AI Agents for Trading | Trading-R1 | RL-trained reasoning LLM on technical and other inputs; arXiv 2509.11420; repository is an API-key terminal client, noted in the entry |

## Observations

- Research code that pairs LLMs with technical indicators is thin. Most matching repositories are prompt-and-indicator wrappers, MCP servers exposing indicators to chat agents, or Pine Script assistants.
- Evidence for vision LLMs reading charts is mixed. An informal public audit of four vision models on QuantAgent-style pattern reading reported near-chance direction accuracy. A 2026 study (arXiv 2605.00875) found that adding indicator overlays degraded CNN chart-based regime prediction. Neither is peer-reviewed, so neither is listed, but readers should treat chart-reading agents with caution.
- Indicator-based RL repositories are mostly older single-paper or course projects (for example, TraderNet-CRv2 and LSTM-PPO traders) with low adoption. FreqAI and the already-listed FinRL, TradeMaster, and gym-anytrading cover this ground better.

## Considered and not added

- **qrak/LLM_trader (Semantic Signal)**: an unusually transparent paper-trading vision-LLM agent, publishing its prompts, memory, and ledger, with 79 indicators. The track record is short (about six weeks) and adoption is low. Revisit.
- **Open-Finance-Lab/AgenticTrading (Agentic Trading Lab)**: an LLM-agent experimentation platform paired with a survey. It is not indicator-specific and has a custom license. Candidate for a general agents pass.
- **pandas-ta-classic, polars_ta, talipp, QuanTAlib, VectorTA, and other indicator libraries**: credible, but the list keeps one or two reference libraries rather than duplicating awesome-quant.
- **TradingView/Pine Script LLM agents (opentrade, PineScript Expert), indicator MCP servers (maverick-mcp, momentum-mcp), Claude "trading skills" packs**: tool wrappers without a research contribution.
- **TraderNet-CRv2, LSTMppo-DRL-StockTrader, CNN candlestick predictors**: older or low-adoption single projects.
- **FinVision (arXiv 2411.08899)**: no official repository located.
