# GitHub sweep: 2026 stock price prediction methods — 2026-11-05

This sweep looked for stock price prediction methods from 2026: repositories created on or after 2026-01-01, and 2026 papers with public code. Thirty GitHub repository searches (`created:>=2026-01-01`) covered stock, return, and trend prediction, cross-sectional ranking, graph, transformer, and Mamba stock models, K-line foundation models, and 2026 venue tags. A literature search for 2026 stock-forecasting papers followed. Repositories already in the list were excluded automatically. Entries were screened against [CONTRIBUTING.md](../../CONTRIBUTING.md), and paper identifiers were checked against arXiv. This is documentation review, not reproduction.

Already in the list from 2026: AlphaPROBE, QuantEvolver, AlphaDiverse, FactorMiner, QuantaAlpha (factor mining), Timestral, Kronos-related work, CAST, and the 2026 LLM benchmarks.

## Added

| Section | Entry | Basis |
| --- | --- | --- |
| Time-Series Foundation Models | KiT | arXiv 2609.34507; flow-matching candlestick model; checkpoint released, training code pending; AGPL-3.0. Deferred in an earlier pass until the paper could be confirmed |
| Research Papers: Forecasting | RankGLU | arXiv 2606.08930; MIT; multi-seed IC results reported honestly (mixed on CSI800) |
| Financial LLM Benchmarks | CrossAlpha | EMNLP 2026 Findings; cross-market annual-report benchmark; MIT |
| Related Lists | TongjiFinLab awesome-time-series-forecasting | Updated October 2026; has a stock price forecasting section; Apache-2.0 |

## Observations

- Few 2026 stock-prediction repositories meet the bar. Repositories created in 2026 that match "stock prediction" are mostly LSTM or Random Forest student projects, Kronos wrappers and agent packaging, and A-share screeners. Research code is the minority and tends to have low star counts.
- The 2026 research directions are candlestick foundation models (KiT, alongside the listed Kronos), better cross-sectional ranking heads and training (RankGLU), text-derived cross-market relations (CrossAlpha), and LLM- or RL-driven factor mining (covered in earlier reviews).
- 2026 papers disagree on whether general foundation models help with financial returns. Summaries of the same 2026 benchmark conflicted, so it is not listed. Earlier evidence, including the NeurIPS 2024 ablation already in the list, is mixed to negative.

## Considered and not added

- **ZJ_Quant_03 (FSQ K-line foundation model and A-share platform)**: an interesting approach (finite-scalar-quantized candlestick tokens), but a single-developer project whose strong backtest figures are self-reported without a paper. Revisit.
- **Pretrained Time-Series Foundation Models for Financial Return Forecasting (arXiv 2606.27100)**: no code, and secondary summaries of its findings conflict. Not listed until the claims can be checked against the full text.
- **Compact selective state-space model for intraday stock ranking (arXiv 2608.28060), consensus-bottleneck asset pricing (CB-APM, a 2025 preprint)**: no 2026 repository, or one with minimal adoption.
- **kit-forecast (Rust port of KiT)**: a community port. The original is listed.
- **Kronos wrappers and agents (kronos-claude-skill, Autotrader, Alpha, cortex-sentinel, RayCodes_Kronos, kronos-guide-cn)**: packaging and demos of an already listed model.
- **end-to-end-stock-transformer, turboquant-qlib, volatility-forecasting horse race, NSE-Neuron, AI-Stock-Predictor, and other LSTM/RF projects**: low adoption or no methodology.
- **FinTSB (TongjiFinLab)**: a credible financial time-series forecasting benchmark, but created in 2024, outside this 2026 pass. Candidate for a general pass.
