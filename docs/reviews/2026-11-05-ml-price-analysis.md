# GitHub sweep: machine learning for stock price analysis and patterns — 2026-11-05

This sweep is the non-LLM companion to the LLM price-analysis review of the same day. It looked for machine-learning methods that predict stock prices or movements and tools that discover price patterns (motifs, regimes, change points, shape similarity). Relevant entries already in the list were excluded: Qlib and its model zoo, ML4T, Gu, Kelly, and Xiu, the image-based price-trend CNN paper, DeepLOB and the LOB benchmark, PatchTST and the other foundation models, alphalens, and the HMM research note. About 30 GitHub repository searches covered graph, transformer, MLP, and drift-adaptive stock models, chart-pattern and support/resistance detection, matrix profiles, change points, DTW clustering, HMM regimes, feature extraction, and time-series deep learning libraries. Entries were screened against [CONTRIBUTING.md](../../CONTRIBUTING.md). Descriptions follow each README, and paper identifiers and authors were checked against arXiv. This is documentation review, not reproduction.

## Added

| Section | Entry | Basis |
| --- | --- | --- |
| Research Environments | STUMPY | Matrix-profile motif and anomaly discovery; JOSS, NumFOCUS |
| Research Environments | ruptures | Change-point detection for regime segmentation; BSD-2-Clause |
| Research Environments | hmmlearn | Standard HMM library for regimes; limited maintenance (noted) |
| Research Environments | tslearn | DTW and shape-based clustering and classification; BSD-2-Clause |
| Research Environments | tsfresh | Automatic feature extraction with relevance filtering; MIT |
| Research Environments | Time-Series-Library (THUML) | Benchmark codebase for deep time-series models; feature freeze noted |
| Research Papers: Forecasting | Temporal Relational Ranking (RSR) | Graph-based stock ranking (arXiv 1809.09441); code and data |
| Research Papers: Forecasting | DoubleAdapt | KDD 2023; online adaptation to distribution shift (arXiv 2306.09862) |
| Research Papers: Forecasting | MASTER | AAAI 2024; market-guided stock transformer (arXiv 2312.15235); MIT |
| Related Lists | stock-top-papers | Top-venue stock-prediction papers with code |

## Observations

- Research-grade stock-prediction models (graph, transformer, MLP, drift-adaptive) mostly come from academic groups that build on Qlib. Their code is usually a cleaned-up release that cannot exactly reproduce the paper; MASTER and DoubleAdapt both say so.
- For "finding patterns" in prices, general time-series tools for motifs, change points, HMM regimes, and DTW are more reliable building blocks than repositories marketed as chart-pattern detectors, which are mostly rule scripts or small YOLO demos with no evaluation.
- Popular "stock prediction" notebooks (for example, LSTM or GAN price forecasting) often predict price levels with look-ahead or trivial persistence baselines. They are excluded as not meeting the list's validation bar.

## Considered and not added

- **borisbanushev/stockpredictionai**: a widely starred notebook with no license and no out-of-sample evaluation methodology.
- **StockMixer (AAAI 2024)**: no license file, from the same group as MASTER. Revisit.
- **HATS, Adv-ALSTM, RTGCN, FinMamba, FactorVAE reimplementations**: older or smaller graph and stock-model codebases, or unofficial implementations. stock-top-papers indexes them.
- **sktime, darts, neuralforecast, tsai, PyPOTS, flow-forecast, functime, tsfel, dtaidistance**: credible general time-series libraries. The list keeps a small set of pattern- and feature-focused ones, and broader forecasting libraries are covered by awesome-quant.
- **ChartScanAI, pytrendline, support/resistance detectors**: small or unevaluated pattern scripts.
- **matrixprofile-ts**: archived. STUMPY is listed instead.
- **Market-regime detection demos, Markov "hedge fund method" skill, XAUUSD bots**: tutorials or bots without methodology.
