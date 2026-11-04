# GitHub sweep — 2026-11-04

Maintainer-initiated search of GitHub for AI/ML quant-finance resources missing from the list. About 40 repository searches (topics `quantitative-finance`, `algorithmic-trading`, `quant`; keyword searches on LLM agents, alpha mining, time-series foundation models, limit order books, deep hedging, portfolio optimization, factor data, benchmarks) were ranked by stars and screened against [CONTRIBUTING.md](../../CONTRIBUTING.md). Descriptions were written from each project's own README and, for papers, the arXiv/proceedings listing. This is documentation review, not independent reproduction.

## Added

| Section | Entry | Basis |
| --- | --- | --- |
| Factor Investing | Open Source Asset Pricing (Chen & Zimmermann) | Peer-reviewed (Critical Finance Review 2022); free data and download packages |
| Factor Investing | JKP Global Factor Data | Journal of Finance 2023; free pre-computed factors at jkpfactors.com |
| HFT | hftbacktest | MIT; latency- and queue-aware L2/L3 backtesting not covered by existing entries |
| HFT | DeepLOB (paper + code) | IEEE TSP 2019; canonical deep LOB model |
| HFT | LOB benchmark study / LOBCAST | Artificial Intelligence Review 2024; negative robustness result is useful due diligence |
| Volatility | Deep Hedging reference implementation (link on existing entry) | Author-maintained code |
| Volatility | PFHedge | MIT; Preferred Networks research code |
| Volatility | arch | Reference GARCH library; baseline for ML volatility forecasts |
| ML and AI Strategies | TradeMaster | NeurIPS 2023 Datasets and Benchmarks; Apache-2.0 |
| ML and AI Strategies | alphalens-reloaded | Maintained fork; maintenance-mode status stated |
| LLM Trading Agents | AI Hedge Fund | MIT; very high adoption; educational/no-live-trading status stated |
| Time-Series Foundation Models | Time-MoE, MOMENT, Sundial | ICLR 2025, ICML 2024, ICML 2025; open weights and code |
| Alpha Mining | AlphaForge | AAAI 2025 official code (no license file in repo) |
| LLM Benchmarks | InvestorBench | ACL 2025; MIT code |
| Strategy Frameworks | PyPortfolioOpt, Cvxportfolio, deepdow | Established/academic portfolio tools; deepdow's quiet maintenance stated |
| Related Lists | financial-machine-learning, awesome-trading-agents | Curated, categorized; slowed updates noted for the former |

## Considered and not added

- **HKUDS/AI-Trader** — now a hosted platform centred on signal sharing, copy trading, and a points system; signal copying is out of scope. No license file.
- **RndmVariableQ/AlphaAgent** — A-share factor framework; not the code for the similarly named KDD paper, and no license file. Revisit if adoption grows.
- **hudson-and-thames/mlfinlab** — public repository unmaintained since 2023; library is now commercial.
- **TradingAgents-CN / TradingAgents-astock / TradingAgents-AShare** — derivatives of an already-listed framework.
- **AutoHedge, QuantDinger, daily_stock_analysis, nof0** — generic LLM wrappers, retail-signal tooling, or competition reproductions without a clear research contribution beyond existing entries.
- **mistralai/timestral** — created 2026-10-15; too new to assess. Revisit.
- **TiRex, Toto, TLOB** — credible, but not added this round to keep sections curated; candidates for a future pass.
- **General trading bots and non-AI platforms** (freqtrade, vnpy, jesse, StockSharp, etc.) — covered by awesome-quant per the scope note.

## Link health of existing entries

Every GitHub repository already linked in the README was checked through the GitHub search API, and none is archived. `OpenBB-finance/OpenBB` now appears on GitHub as `openbq-org/OpenBB` (same repository, created 2020-12-20), and the old URL still resolves. The link was left unchanged until the maintainer confirms the new organization name.
