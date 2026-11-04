# GitHub sweep: repositories created in 2026 — 2026-11-04

Second pass of the same day's sweep. This one is limited to repositories **created on or after 2026-01-01** that apply LLMs, reinforcement learning, or other ML to quantitative finance. About 55 searches (`created:>=2026-01-01`) covered trading agents, alpha/factor mining, RL for portfolios, execution, market making and options, GRPO/RLVR, financial benchmarks, time-series foundation models, order books, and prediction markets. Results were ranked by stars and screened against [CONTRIBUTING.md](../../CONTRIBUTING.md). Descriptions follow each project's README. Paper IDs were checked against arXiv or ACL Anthology search listings. This is documentation review, not reproduction.

## Added

| Section | Entry | Basis |
| --- | --- | --- |
| LLM-Based Trading Agents | TraderHarness | Apache-2.0; addresses LLM training-data leakage in agent backtests, a gap in the list |
| Time-Series Foundation Models | Timestral (Mistral AI) | Major-lab release with open weights; rankings marked vendor-reported |
| AI-Driven Alpha Mining | QuantaAlpha | arXiv 2602.07085; high adoption; no license file (noted) |
| AI-Driven Alpha Mining | FactorMiner | arXiv 2602.14670; MIT |
| Financial LLM Benchmarks | FinMTM | arXiv 2602.03130; MIT dataset on Hugging Face |
| Financial LLM Benchmarks | FinMRAGBench | ACL 2026 Findings |
| Financial LLM Benchmarks | CNFinBench | Shanghai AI Lab / OpenCompass; arXiv 2512.09506 (repository created 2026) |
| On-Chain / DeFi | Polymarket Data | Academic dataset (1.1B records), MIT, Hugging Face |
| Strategy Development Frameworks | AKQuant | MIT; AKShare team; built-in walk-forward ML |
| Research Papers: AI Agents for Trading | SOTA (options, SFT + RL) | CMU/Amazon preprint with MIT code; linked to the PDF in the repository because the arXiv listing was only seen in secondary sources |

## Observations

- **Reinforcement learning:** few 2026 repositories apply RL to trading with any traction. The searches for execution, market making, options, and GRPO returned mostly coursework and thesis projects with single-digit stars. SOTA was the only RL work that met the bar.
- **LLM agents:** much of the 2026 volume is A-share retail tooling, TradingAgents derivatives, agent "skills" packs, and prediction-market bots.

## Considered and not added

- **KiT** (candlestick diffusion foundation model): the arXiv ID could not be confirmed outside a secondary blog post, and training code is not yet released. Revisit.
- **imbue-bit/AlphaGPT**: the README contains no technical documentation, only donation and dispute notices.
- **OpenAlice, ALTA, LangAlpha, Vibe-Research**: agent research workspaces. Adoption is real, but they don't yet add a distinct research contribution over the listed agent frameworks.
- **atlas-gic**: self-improvement claims and "live with real capital" with no public evaluation methodology. Custom license.
- **Loopera**: product-description repository with no runnable code.
- **qsx-strategy-score**: funnels to a hosted commercial scorer.
- **QuantGPT, worldquant-miner and similar**: automation for WorldQuant BRAIN submissions.
- **PolyBench, PredictionMarketBench, QF-Bench, FinVault**: promising agent benchmarks, but with no confirmed paper or very low adoption so far. Revisit.
- **daily_stock_analysis, PanWatch, TradingAgents-astock/AShare, CloddsBot, Polymarket/Kalshi bots**: retail alerting, forks, or execution bots outside scope.
- **TS-ICL, CogAlpha**: TS-ICL is a general-purpose forecasting model, and CogAlpha has only a prompt-template repository. Revisit when finance-specific results or full code are released.
