# GitHub sweep: learning to use LLMs for trading — 2026-11-05

This targeted sweep looked for resources that teach how to use LLMs for trading and investment research: tutorials, notebooks, courses, books with code, official reference implementations, surveys, and paper lists. About 60 GitHub repository searches were combined with lookups of known books and surveys, and repositories already in the list were excluded automatically. Entries were screened against [CONTRIBUTING.md](../../CONTRIBUTING.md). Descriptions follow each README. Book authors were checked against publisher listings and paper identifiers against arXiv. This is documentation review, not reproduction.

## Added

| Section | Entry | Basis |
| --- | --- | --- |
| Learning Resources | LLMs-in-Finance | Hands-on notebooks across agent frameworks, RAG, and multimodal; MIT |
| Learning Resources | AI Quant Trading: From Zero to One | Free bilingual book (22 lessons) on agent-based trading systems; CC BY-NC-SA 4.0 |
| Learning Resources | Introduction to Quantitative Finance (Barca0412) | Chinese knowledge base with an AI + Finance arXiv radar; MIT |
| Learning Resources | Claude for Financial Services (Anthropic) | Official reference agents and skills; research and analyst workflows, not trading (noted); Apache-2.0 |
| Books | Generative AI for Trading and Asset Management | Medina Ruiz and Chan, Wiley 2025; notebook repository |
| Books | Hands-On AI Trading with Python, QuantConnect, and AWS | Pik, Chan, Broad, Sun, and Singh, Wiley 2025; runnable LLM and FinBERT examples |
| Research Papers: LLMs in Finance | FinLLMs survey | arXiv 2402.02315; companion resource list |
| Research Papers: AI Agents | LLM agents in financial trading survey | arXiv 2408.06361 |
| Research Papers: AI Agents | CryptoTrade | EMNLP 2024; official code |
| Related Lists | Awesome LLM Quantitative Trading Papers | Organized paper list with a curation policy |

## Observations

- Good LLM-for-trading teaching material is scarce. Most "tutorial" repositories are single LangChain or LangGraph demos, agent "skill" packs, or Udacity nanodegree solution copies that predate LLMs.
- The strongest practical material sits in books with code (Wiley 2025 titles co-authored by Ernest Chan) and in notebook collections such as LLMs-in-Finance. The best orientation comes from surveys.

## Considered and not added

- **Udacity AI for Trading** (course content and many student solution forks): pre-LLM and no longer updated.
- **hands-on-llms (Decoding ML)**: a financial-advisor LLMOps course, archived in 2024.
- **LLMQuant/quant-wiki**: a broad Chinese quant wiki, not LLM-specific.
- **Awesome-finance-skills, finance_skills, claude-for-financial-services-cn, awesome-finance-mcp**: agent skill packs and connector lists without a research contribution.
- **DataArcTech/Awesome-FinLLMs, AI4Finance Awesome_AI4Finance, LLM_X_papers**: lower-maintenance paper lists, overlapping with lists already linked.
- **Agentic_FinTech_Survey, awesome-applied-agents-for-investment**: very new with low adoption. Revisit.
- **LLM-RAG_Finance_UseCases, 100-AI-Agents projects, LangGraph course repositories**: generic or not trading-focused.
