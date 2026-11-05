# GitHub sweep: using LLMs in quant jobs — 2026-11-05

This sweep looked for resources on how quant researchers, traders, and developers use LLMs in day-to-day industry work: coding agents for research, guardrails against leakage, LLM access to filings and research platforms, and preparation for quant roles. About 30 GitHub repository searches covered quant research assistants, agent skills, SEC filings for LLMs, research-platform MCP servers, data-analysis agents, and interview preparation. Repositories already in the list were excluded automatically. Entries were screened against [CONTRIBUTING.md](../../CONTRIBUTING.md), and descriptions follow each README. This is documentation review, not reproduction.

## Added

| Section | Entry | Why |
| --- | --- | --- |
| Learning Resources | Agentic AI in Trading (ML4T workshop) | Shows, with captured runs and an audit notebook, how to supervise a coding agent doing quant research, plus a six-point checklist; MIT |
| Learning Resources | ML4T Agent Skills | 61 skills that put leakage, look-ahead, and validation discipline into coding agents; Apache-2.0 |
| Learning Resources | Quant-Developers-Resources | Widely used preparation guide for quant roles; no license file (noted) |
| Data Providers | EdgarTools | Free SEC filings as structured data, with an agent skill and MCP server; MIT |
| Execution & Deployment | QuantConnect MCP Server | Official way to drive research, backtests, and deployment from AI assistants; paid agent node required (noted) |

## Observations

- The practical lesson across these resources is supervision, not autonomy. Coding agents write plausible research pipelines quickly, and the value is in checks for leakage, look-ahead, and multiple testing. The ML4T workshop shows four runs of the same task answering the research question correctly but returning different amounts of evidence.
- Most "AI quant assistant" repositories are thin LLM wrappers, MCP connectors to retail data, or A-share "skill" packs. CONTRIBUTING.md excludes connectors without a research contribution unless they come from the platform owner (QuantConnect) or a widely used data library (EdgarTools).

## Considered and not added

- **pandas-ai, DeepAnalyze, deep-searcher**: general data-analysis and research agents, not finance-specific.
- **AgentQuant, open-xquant, AlphaResearchOS, EvoQuant, alphaevo**: agentic quant research harnesses that are promising but early, with low adoption and no paper. Revisit.
- **QuantGPT (rnikitin), quantcoder (archived), quantconnect-mcp (unofficial)**: unmaintained or superseded by the official QuantConnect server.
- **sec-edgar-mcp, yahoo-finance-mcp, maverick-mcp, metatrader-mcp-server, Wind AliceMarket, quantskills and A-share skill packs**: connectors and skill packs without a research contribution.
- **sec-edgar, sec-edgar-downloader, sec-api-python**: filing downloaders. EdgarTools is the more complete, LLM-ready option.
- **Trading-Interview-Questions, QuantitativePrimer, quant-notes, awesome-quant-interview, ML-Interview**: smaller or older interview guides. One comprehensive guide is listed.
- **Interview-copilot tools (for example, Natively)**: out of scope.
