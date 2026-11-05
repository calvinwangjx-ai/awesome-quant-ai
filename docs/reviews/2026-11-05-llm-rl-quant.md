# GitHub sweep: LLMs and reinforcement learning for quant trading — 2026-11-05

This general sweep, with no date restriction, aimed to fill gaps left by the earlier targeted passes (alpha mining, indicators, 2026-only). It covered about 40 GitHub repository searches on RL trading frameworks and gym environments, RL for portfolios, execution and market making, order-book and agent-based simulators, financial reasoning LLMs, LLM market simulations, live LLM trading arenas, and reproducibility work. Repositories already in the list were excluded automatically. Entries were screened against [CONTRIBUTING.md](../../CONTRIBUTING.md), descriptions follow each README, and paper identifiers were checked against arXiv listings. This is documentation review, not reproduction.

## Added

| Section | Entry | Basis |
| --- | --- | --- |
| HFT | mbt_gym | ICAIF 2023; BSD-3-Clause; RL environments for market making and execution with analytical benchmarks |
| HFT | ABIDES | Reference agent-based market simulator (arXiv 1904.12066); unmaintained since 2023 (noted) |
| ML and AI Strategies | TensorTrade | Apache-2.0; long-standing RL trading framework |
| ML and AI Strategies | FinRL-Meta | MIT; market environments and datasets for financial RL (arXiv 2304.13174) |
| ML and AI Strategies | FinRL-DeepSeek | MIT; LLM signals into risk-sensitive RL (arXiv 2502.07393); preliminary results (noted) |
| ML and AI Strategies | PGPortfolio | Canonical deep-RL portfolio paper code; README's own test-period caveat noted; unmaintained |
| LLM-Based Trading Agents | TwinMarket | NeurIPS 2025; MIT; LLM multi-agent market simulation |
| AI-Driven Alpha Mining | Alpha-R1 | RL-trained (GRPO) alpha-screening LLM with released weights; arXiv 2512.23515 (deferred from the 2026-only pass because the repository dates from December 2025) |
| Financial LLM Benchmarks | Agent Market Arena | The FinAI; live multi-market LLM trading benchmark (arXiv 2510.11695); MIT |
| Financial LLM Benchmarks | RL-pricing | Pre-registered re-tests of published RL and LLM trading claims; MIT; early-stage (noted) |
| Diffusion / Synthetic Data | MarS (Microsoft) | ICLR 2025; MIT; generative order-flow simulation with released order models |
| Research Papers: LLMs in Finance | Fin-R1 | SFT + GRPO financial reasoning model; arXiv 2503.16252; weights released |
| Research Papers: AI Agents | FinMem | Added the official code link to the existing entry |

## Observations

- Most RL trading repositories on GitHub are 2017-2020 single-paper or course projects (DQN/DDPG stock traders, gym wrappers), and most are unmaintained. Of that generation, only the frameworks with continuing use (TensorTrade, FinRL and FinRL-Meta) and the canonical PGPortfolio code are listed.
- The most useful new LLM resources are about **evaluation hygiene**: live arenas (Agent Market Arena) and pre-registered re-tests (RL-pricing). They address look-ahead and memorization in LLM backtests, which TraderHarness also targets.
- Reinforcement learning in LLM finance work now mostly means post-training the model (Fin-R1, Alpha-R1, Trading-R1, QuantEvolver), not training classic RL trading policies.

## Considered and not added

- **ElegantRL**: a general massively parallel DRL library, not finance-specific. FinRL already covers its finance use.
- **JAX-LOB / AlphaTrade (Oxford)**: a relevant GPU order-book simulator for RL (ICAIF 2023), but the repository README is a weekly research log with no license. Revisit if a packaged release appears.
- **abides-jpmc-public**: J.P. Morgan's gym-enabled ABIDES fork is archived. The original ABIDES is listed instead.
- **Agentic Trading Lab (Open-Finance-Lab)**: an LLM-agent experimentation platform with a custom lab license and a hosted leaderboard. Revisit when its survey paper and license terms are clearer.
- **nof0, Super-nof1.ai, crypto-trading-arena, botstreet, and other "Alpha Arena" reproductions**: no license, or demos without an evaluation methodology.
- **DISC-FinLLM, finance DeepSeek-R1 fine-tuning guides**: dated (2023) or tutorial-level.
- **Gym-Trading-Env, TradingGym, RLTrader, deep_trader, Personae, and similar**: simple or unmaintained environments, superseded by listed frameworks.
- **HFTFramework**: thesis code for RL-enhanced Avellaneda-Stoikov market making. It is credible, but mbt_gym covers the area with a peer-reviewed, packaged suite.
- **StockSim, ai-hedge-fund-crypto, CryptoTradingAgents, TradingGoose**: low adoption, or derivatives of listed frameworks.
