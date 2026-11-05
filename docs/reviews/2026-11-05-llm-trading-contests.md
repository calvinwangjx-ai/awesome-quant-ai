# GitHub sweep: LLM trading contests, arenas, and live benchmarks — 2026-11-05

This targeted sweep covered contests, live arenas, and benchmarks where LLM (and ML/RL) trading agents compete or are scored on markets. Thirty GitHub repository searches (Alpha Arena and nof1, trading arenas and leaderboards, FinRL, ICAIF and SecureFinAI contests, prediction-market arenas, Numerai, quant competitions) were combined with a literature search for live trading benchmarks with code. Entries were screened against [CONTRIBUTING.md](../../CONTRIBUTING.md). Descriptions follow each README or official page, and paper identifiers come from the repositories or arXiv listings. This is documentation review, not reproduction.

A new **Competitions** subsection was added under Community and Conferences, because no existing section fit recurring contests.

## Added

| Section | Entry | Basis |
| --- | --- | --- |
| Competitions | Alpha Arena (Nof1) | The reference live real-money LLM trading contest; organizer caveats on luck and sample size are stated |
| Competitions | FinRL Contests | Annual ACM ICAIF contests (2023-2025) combining RL and LLM tasks; starter kits on GitHub |
| Competitions | ICAIF 2026 Trading Agent Competition | Official ICAIF 2026 competition; starter kit repository |
| Competitions | Numerai | Long-running crowdsourced ML tournament; MIT example scripts |
| Financial LLM Benchmarks | LiveTradeBench | UIUC; arXiv 2511.03628; live stocks and Polymarket evaluation; PolyForm Noncommercial (noted) |
| Financial LLM Benchmarks | StockBench | arXiv 2510.02209; Apache-2.0; post-2024 data to limit contamination |
| Financial LLM Benchmarks | AlphaForgeBench | HKUST(GZ); arXiv 2602.18481; MIT; LLM strategy-code generation scored by backtests |
| Financial LLM Benchmarks | Prophet Arena | arXiv 2510.17638; live prediction-market forecasting benchmark (no official repository located) |
| LLM-Based Trading Agents | Agent Trading Arena | EMNLP 2025 Findings; follow-up DecoupledMarket (ICML 2026) |

Already listed and relevant to this topic: Agent Market Arena, RL-pricing, TraderHarness, and FinRL-DeepSeek (a FinRL Contest 2025 task).

## Observations

- After Nof1's Alpha Arena (October 2025), GitHub filled with clones: nof0, open-nof1.ai, open-alpha-arena, Alpha-Arena-Lite, and many exchange-specific forks. Most have no license, and several copy-trade the arena's public positions. Only the original contest is listed, with nof0 mentioned as a reproduction.
- The research benchmarks converge on the same lesson: **live or post-cutoff evaluation is necessary**, because historical backtests of LLM agents are exposed to training-data memorization. LiveTradeBench also reports that general reasoning scores do not predict trading results.
- Contest results are noisy. Alpha Arena's organizers attribute early rankings partly to luck, and the press coverage reported inconsistent figures, so no season results are quoted in the list.

## Considered and not added

- **nof1-tracker, alpha-arena-okx, Hyper-Alpha-Arena, open-nof1.ai, OpenNof1, Super-nof1.ai, and similar**: Alpha Arena clones or copy-trading tools. Copy trading is out of scope, and most have no license.
- **kukapay/awesome-alpha-arena**: a small list of clones, superseded by linking the original.
- **SecureFinAI Contest (2025, 2026)**: a related Open Finance Lab contest focused on secure and reliable financial AI. It is reachable through the FinRL Contest documentation, so it is not listed separately.
- **OpenFinArena**: challenges for LLM financial analysis and forecasting, not trading. It has no license. Candidate for a benchmarks pass.
- **"Perpetual Alpha" (ICAIF 2026, Hyperliquid testnet)**: seen only in a mailing-list announcement and not confirmed on an official page.
- **crypto-trading-arena, wtfibought, botstreet, agenttrader-arena, AURA Arena, AgentStockBenchmarkResults, and similar live arenas**: low adoption, no paper or methodology.
- **Kaggle and university trading-competition solutions (Jane Street, Optiver, Akuna, Citadel, Cornell)**: individual solution repositories, not resources. Not LLM-specific.
- **Quant-Arena (arXiv 2610.30113)**: no repository located.
