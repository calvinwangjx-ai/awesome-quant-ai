# GitHub sweep: LLMs for stock price analysis and price patterns — 2026-11-05

This targeted sweep looked for resources on using LLMs to analyze stock prices and find price patterns. Relevant entries already in the list were excluded: Kronos, Chronos, TimesFM, and the other time-series foundation models, QuantAgent's chart-pattern agent, and the image-based price-trend paper (Jiang, Kelly, and Xiu). About 40 GitHub repository searches covered LLM stock-movement prediction, LLMs reading price series as text, LLM time-series reasoning, retrieval of similar price patterns, explainable prediction, and stock-movement datasets. Lookups of known papers followed. Entries were screened against [CONTRIBUTING.md](../../CONTRIBUTING.md). Descriptions follow each README, and paper identifiers were checked against arXiv. This is documentation review, not reproduction.

## Added

| Section | Entry | Basis |
| --- | --- | --- |
| Time-Series Foundation Models | LLMTime | NeurIPS 2023; numbers as text with a general LLM; MIT |
| Time-Series Foundation Models | Time-LLM | ICLR 2024; reprogramming a frozen LLM; Apache-2.0 |
| Time-Series Foundation Models | ChatTS | VLDB 2025; LLM with native time-series input for Q&A and reasoning; 14B model released; MIT |
| Time-Series Foundation Models | Are Language Models Actually Useful for Time Series Forecasting? | NeurIPS 2024 Spotlight; negative ablation result |
| Research Papers: LLMs in Finance | FinSeer | Retrieval of relevant historical price sequences for LLM forecasting (arXiv 2502.05878); MIT |
| Research Papers: LLMs in Finance | SEP | Explainable stock prediction with self-reflection and PPO fine-tuning (arXiv 2402.03659) |
| Financial LLM Benchmarks | StockNet | ACL 2018 tweet-and-price movement dataset; contamination caveat noted |
| Related Lists | Awesome-TimeSeries-SpatioTemporal-LM-LLM | Main LLM-for-time-series paper list (inactive since 2024, noted) |
| Related Lists | Transformers_And_LLM_Are_What_You_Dont_Need | Counter-evidence collection |

## Observations

- The evidence that LLMs find exploitable price patterns is weak. The NeurIPS 2024 ablation study, the counterpoint collection, and earlier findings (the vision-LLM chart audit and LiveTradeBench, recorded in prior reviews) all point the same way. The more defensible uses are reasoning over text alongside prices (SEP), retrieving comparable historical episodes (FinSeer), or dedicated numeric foundation models (Kronos, Chronos) rather than general chat LLMs.
- Older benchmarks such as StockNet (2014-2016) likely overlap LLM pre-training data, so strong results on them may reflect memorization.
- The most-starred "LLM stock analysis" repositories are daily report and notification tools, not research.

## Considered and not added

- **daily_stock_analysis** (very high adoption): an LLM daily "decision dashboard" with buy/sell points pushed to chat apps, plus a model-API reseller sponsorship. It is a retail alerting tool with no evaluation methodology, which CONTRIBUTING.md excludes. **easy-stock, PanWatch, Nova-TradingAgent, WyckoffTradingAgent, EOD-GPT, stock-daily-analysis-skill** were excluded for similar reasons.
- **TimeCopilot**: an agentic forecasting framework combining LLMs and foundation models. It is credible but general-purpose rather than finance-specific. Revisit.
- **LLM4TS (aligned LLM forecaster), TimeCMA, CALF, UniTime**: general LLM forecasting methods already covered by Time-LLM and the ablation study.
- **TimeMaster, Time-Series-Reasoning-Survey, HEARTS**: general time-series reasoning work that is not finance-specific.
- **ChatGPT-GNN-StockPredict, GPT-InvestAR, Ploutos reimplementations**: small or unofficial projects.
- **liaoyuhua/LLM4TS paper list**: overlaps with the listed time-series LLM list.
