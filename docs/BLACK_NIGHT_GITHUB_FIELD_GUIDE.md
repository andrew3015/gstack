# Black Night Finance Studio — GitHub Field Guide

A curated, practical directory of open-source projects and engineering references to evaluate for Black Night Finance Studio. This is a research shortlist, not a claim that every project is installed, compatible, free to operate, or safe to run. Review licenses, maintenance, security, hardware requirements, and dependencies before adoption.

## Start here: the two engineering references

### Matt Pocock — `@mattpocock`
- GitHub: https://github.com/mattpocock
- Skills: https://github.com/mattpocock/skills — reusable instructions and workflows for coding agents.
- Sandcastle: https://github.com/mattpocock/sandcastle — sandboxed/parallel coding-agent orchestration.
- Evalite: https://github.com/mattpocock/evalite — evaluation tooling for AI applications.
- TypeScript Reset: https://github.com/mattpocock/ts-reset — TypeScript type-safety utilities.
- AI coding dictionary: https://github.com/mattpocock/dictionary-of-ai-coding
- YouTube: https://www.youtube.com/@mattpocockuk
- LinkedIn: https://www.linkedin.com/in/mapocock/
- Website: https://www.mattpocock.com/
- AI Hero: https://aihero.dev/
- Total TypeScript: https://www.totaltypescript.com/

**Study for Black Night:** agent instructions, safe execution boundaries, evaluation tests, TypeScript quality, and repeatable engineering workflows.

### Lauren Tan — `@poteto`
- GitHub: https://github.com/poteto
- pstack (Cursor plugin repository): https://github.com/cursor/plugins/tree/main/plugins/pstack
- X: https://x.com/poteto
- LinkedIn: https://www.linkedin.com/in/laurenelizabethtan/
- Personal site/blog: https://www.no.lol/

**Study for Black Night:** coordinated coding-agent workflows, delegation, pull-request review, and engineering practices. Verify the current repository and project ownership before attributing any third-party project to Lauren personally.

## High-priority open-source projects to evaluate

### Agent frameworks and orchestration
1. OpenClaw — https://github.com/openclaw/openclaw — personal/assistant agent framework; inspect permissions and security model carefully.
2. LangGraph — https://github.com/langchain-ai/langgraph — stateful, graph-based agent workflows.
3. PydanticAI — https://github.com/pydantic/pydantic-ai — typed Python agent framework.
4. Microsoft AutoGen — https://github.com/microsoft/autogen — multi-agent application framework.
5. CrewAI — https://github.com/crewAIInc/crewAI — role-based multi-agent orchestration.
6. Hermes Agent — https://github.com/NousResearch/hermes-agent — local/hosted agent runtime and tool workflows; compare with the existing Hermes setup rather than duplicating it.

### Coding agents and software factories
1. gstack — https://github.com/garrytan/gstack — structured roles and workflows for planning, review, QA, security, and shipping.
2. OpenHands — https://github.com/All-Hands-AI/OpenHands — software-development agent platform.
3. SWE-agent — https://github.com/SWE-agent/SWE-agent — agent workflows for software engineering issues.
4. Aider — https://github.com/Aider-AI/aider — terminal-based AI pair programming.
5. Continue — https://github.com/continuedev/continue — open-source AI coding assistant and IDE integration.
6. Cline — https://github.com/cline/cline — autonomous coding assistant with tool permissions.
7. Roo Code — https://github.com/RooCodeInc/Roo-Code — coding-agent workflows and modes.

### Local models, inference, and model routing
1. Ollama — https://github.com/ollama/ollama — run supported models locally.
2. llama.cpp — https://github.com/ggml-org/llama.cpp — efficient local inference across supported hardware.
3. vLLM — https://github.com/vllm-project/vllm — high-throughput inference; likely better suited to stronger hardware than the current desktop.
4. LiteLLM — https://github.com/BerriAI/litellm — unified model/provider routing and spend controls.
5. Hugging Face Transformers — https://github.com/huggingface/transformers — model loading and inference ecosystem.

### Browser automation, integrations, and tool protocols
1. Playwright — https://github.com/microsoft/playwright — reliable browser automation and end-to-end tests.
2. Browser Use — https://github.com/browser-use/browser-use — browser automation for AI agents.
3. Model Context Protocol (MCP) specification — https://github.com/modelcontextprotocol/modelcontextprotocol — standard for connecting tools and data sources.
4. Official MCP servers — https://github.com/modelcontextprotocol/servers — reference integrations; review each server's permissions and maintenance.

### Evaluation, observability, and security
1. Inspect AI — https://github.com/UKGovernmentBEIS/inspect_ai — evaluation framework.
2. promptfoo — https://github.com/promptfoo/promptfoo — prompt/model testing and red-team evaluations.
3. Langfuse — https://github.com/langfuse/langfuse — LLM tracing and observability.
4. OpenTelemetry — https://github.com/open-telemetry/opentelemetry — vendor-neutral telemetry.
5. Semgrep — https://github.com/semgrep/semgrep — static analysis and security scanning.
6. Trivy — https://github.com/aquasecurity/trivy — vulnerability and configuration scanning.
7. OWASP Juice Shop — https://github.com/juice-shop/juice-shop — intentionally vulnerable app for safe security-learning labs.

### Data, finance, and research foundations
1. DuckDB — https://github.com/duckdb/duckdb — embedded analytical database.
2. Polars — https://github.com/pola-rs/polars — fast dataframe processing.
3. Pandas — https://github.com/pandas-dev/pandas — data analysis toolkit.
4. SEC EDGAR APIs — https://www.sec.gov/edgar/sec-api-documentation — official filing data documentation (not a GitHub project).
5. OpenBB — https://github.com/OpenBB-finance/OpenBB — financial data and research platform; verify data-provider terms and availability.
6. QuantLib — https://github.com/lballabio/QuantLib — quantitative finance library.

## Recommended adoption order for this desktop

The current desktop has limited RAM and integrated graphics. Favor lightweight tools and hosted/free tiers only when needed; don't try to run large models or heavyweight services locally by default.

1. **Inventory first:** map existing Hermes, REA MCP, Python, model cache, and G: drive setup. Avoid installing duplicate runtimes.
2. **Agent quality:** borrow Matt's skills/evaluation patterns; define role prompts, test cases, and acceptance criteria.
3. **Workflow design:** study Lauren's pstack approach and gstack's role-based workflow; create supervisor, finance research, job search, grants, coding, QA, and security roles.
4. **Safe browser work:** evaluate Playwright first; require explicit approval before purchases, submissions, account changes, messages, or other consequential actions.
5. **Model routing:** compare Ollama/llama.cpp for small local models and LiteLLM for routing; keep model and cache files on G:.
6. **Observability and security:** log tool calls, source URLs, timestamps, model, cost, outputs, approvals, and errors; add promptfoo/Inspect AI tests and Semgrep/Trivy checks.
7. **Finance data:** use official sources and documented APIs; preserve provenance, timestamps, licensing/terms, and reconciliation checks.

## Non-negotiable safeguards

- Do not run install scripts, downloaded binaries, containers, MCP servers, or browser extensions without reviewing their source, permissions, and publisher.
- Pin versions and record the commit/release used; don't blindly follow a repository's latest branch.
- Keep secrets out of Git. Use environment variables or a secrets manager; never commit API keys, passwords, tokens, personal financial data, or credentials.
- Use least-privilege access and isolated workspaces for coding agents.
- Require human approval for money movement, purchases, financial transactions, job applications, legal filings, public posts, deleting data, or changing account/security settings.
- Treat repository stars and follower counts as popularity signals, not proof of quality, safety, maintenance, or suitability.
- Record license, last release/commit, open security advisories, supported platforms, and hardware needs before adoption.

## Review checklist for each candidate

- [ ] Confirm official owner and repository URL.
- [ ] Check license and commercial-use implications.
- [ ] Check recent commits, releases, issues, and maintainer activity.
- [ ] Review dependencies, install scripts, permissions, and security advisories.
- [ ] Test in a disposable environment before connecting credentials or production data.
- [ ] Measure RAM, disk, CPU/GPU, latency, and operating cost.
- [ ] Decide: adopt, pilot, watch, or reject; record why.

---
Last curated: 2026-11-10. Re-check repository activity, versions, licenses, and security before installation.
