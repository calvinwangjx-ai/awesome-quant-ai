# GitHub sweep: current working trading strategies and alphas — 2026-11-05

This sweep set out to find "currently working" strategies and alphas on GitHub. It started from a caveat: an edge that is published or open-sourced tends to decay as capital arbitrages it away, and verifiable live performance is rarely public. So the sweep looked for (1) strategy replications that keep re-running results after publication, (2) research measuring how published alphas decay, (3) regularly updated factor-return data, and (4) reference strategy and alpha catalogs, labelled honestly. About 30 GitHub repository searches (strategy libraries, Alpha101/191, anomaly and factor replications, broker-report replications, trend, carry, momentum, mean reversion, stat arb, options, crypto) were combined with literature lookups. Repositories already in the list were excluded automatically. Paper identifiers and headline statistics were checked against the published abstracts. This is documentation review, not reproduction.

## Added

| Section | Entry | Why |
| --- | --- | --- |
| Factor Investing | McLean and Pontiff (JF 2016) | Measured decay: −26% out-of-sample, −58% post-publication across 97 predictors |
| Factor Investing | Hou, Xue, and Zhang, Replicating Anomalies (RFS 2020) | 65% / 82% of 452 anomalies fail t = 1.96 / 2.78 |
| Factor Investing | 101 Formulaic Alphas (Kakushadze 2016) | Canonical public alpha set, framed as a baseline, not a live edge |
| Factor Investing | AQR Data Sets | Free, regularly updated returns of published factors, for checking post-publication performance |
| Trend Following | A Century of Evidence on Trend-Following Investing (JPM 2017) | Long-horizon robustness evidence for one of the more persistent premia |
| Trend Following | rolling-panda-san/notebooks | Published futures strategies re-run and pushed regularly; private data library noted |
| Learning Resources | QuantsPlaybook | 100+ Chinese broker-report strategy replications; no license file (noted) |
| Learning Resources | quant-trading (je-suis-tm) | Readable classic strategy implementations; labelled educational |
| Research Papers (existing) | Deep Learning Statistical Arbitrage | Added the official code link |

## Observations

- No reputable public repository demonstrates a live, currently profitable alpha with audited out-of-sample results. Repositories claiming "working" or "profitable" strategies typically show in-sample backtests.
- The most useful evidence on what still works is post-publication tracking: the regularly re-run replications (rolling-panda-san), AQR's updated factor series, and the decay literature above. Earlier entries already in the list cover the same ground: the JKP factor data and Open Source Asset Pricing, the "factor zoo" critique (Harvey, Liu, and Zhu), and RL-pricing's pre-registered re-tests.

## Considered and not added

- **151 Trading Strategies (Kakushadze and Serur)**: Springer's listing marks the Palgrave book as retracted, so it is excluded despite the free SSRN version. Implementations such as `strategist` were excluded with it.
- **NostalgiaForInfinity and other Freqtrade or crypto bot strategies (MoniGoMani, Gekko-Strategies, grid/DCA bots)**: community-run strategies whose performance claims are anecdotal or in-sample. Out of scope for "documented" strategies.
- **The-Quant-Trading-Vault ("5800+ strategies") and similar bulk collections**: no evidence or provenance.
- **Alpha101/Alpha191 code repositories (yli188, STHSF, popbo, 101_formulaic_alphas)**: implementations of the paper above. Qlib and AKQuant already ship these feature sets.
- **smart-money-concepts (ICT indicators), fmzquant/strategies, finmarketpy, hikyuu, backtesting.py**: indicator libraries, strategy marketplaces, or general backtesters rather than evidence about strategies.
- **ai_quant_trade, QuantDinger**: broad platforms, not evidence about strategies.
- **Pairs-trading and stat-arb student projects, TSMOM single replications**: low adoption. rolling-panda-san covers TSMOM with ongoing updates.
- **Carry (Koijen, Moskowitz, Pedersen, and Vrugt)**: relevant, but its identifier was not confirmed in this pass. Revisit.
