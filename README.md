# Awesome-AI-Observability-Evaluation

# Top AI Observability & Evaluation Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on LLM Tracing, Automated Scoring & Production Quality Monitoring*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Observability & Evaluation**. These tools give teams visibility into every LLM call, agent step, and retrieval decision—scoring outputs automatically, detecting quality drift, and catching regressions before users notice.

**Examples** include Arthur AI, Fiddler, Arize AI, WhyLabs, TruEra, Patronus AI, Braintrust, LangSmith, Galileo, and Humanloop (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, OpenTelemetry-native tracing, and open evaluation frameworks—ideal for ML engineers, platform teams, and developers seeking transparent, vendor-independent observability.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Arthur AI](https://www.arthur.ai/)**  
  Enterprise AI observability and evaluation platform. Features **Arthur Shield** for real-time guardrails, **Arthur Bench** for offline evaluation, and **Arthur Engine** for production monitoring. Detects hallucinations, toxicity, PII leakage, and performance drift.

- **[Fiddler AI](https://www.fiddler.ai/)**  
  Enterprise AI observability with explainability, bias detection, and LLM evaluation. **Experiments** feature supports A/B testing prompts, model version comparison, regression testing, safety validation, and RAG system evaluation using RAG Health Metrics (AnswerRelevance, ContextRelevance, RAGFaithfulness).

- **[Arize AI](https://arize.com/)**  
  Enterprise AI observability platform with production-scale telemetry and 50+ research-backed eval metrics. **Arize Phoenix** is the open-source counterpart under Elastic 2.0 license. Unified ML + LLM observability.

- **[WhyLabs](https://whylabs.ai/)**  
  AI observability platform with statistical profiling, drift detection, and performance monitoring. **WhyLogs** open-source library for data logging.

- **[TruEra](https://truera.com/)**  
  AI quality management platform with testing, monitoring, and explainability. **Acquired by Snowflake (2024)**.

- **[Patronus AI](https://www.patronus.ai/)**  
  **Hosted evaluation API with configurable evaluators** for hallucination (Lynx), toxicity, PII, prompt injection, and custom judging. Single `/v1/evaluate` endpoint runs multiple evaluators per request with pass/fail verdicts and explanations. **Free Developer tier**.

- **[Braintrust](https://www.braintrust.dev/)**  
  **Eval-first observability platform with CI/CD quality gates.** Trusted by Notion, Stripe, Vercel, Dropbox, and Coursera. **Freemium**: Starter free (1 GB logs/month, 14-day retention, 10k eval runs/month), Pro at $249/month.

- **[LangSmith](https://smith.langchain.com/)**  
  LangChain's observability and evaluation platform with detailed tracing of every LLM call, chain execution, and agent step. **Free Developer plan** (1 seat, 5k base traces/month), **Plus at $39/seat/month**.

- **[Galileo](https://galileo.ai/)**  
  Enterprise AI evaluation and observability platform with Experiments API, Groups API, and Integrations API. Systematic evaluation workflows for production AI systems.

- **[Humanloop](https://humanloop.com/)**  
  LLM Evals Platform for Enterprises with prompt engineering, evaluation, and observability. **Free tier**: 2 members, 50 eval runs, 10K logs/month.

## Open-Source GitHub Projects

- **[Arize Phoenix](https://github.com/Arize-ai/phoenix)**  
  **The most widely adopted open-source AI observability and evaluation platform for LLMs and generative apps** (Elastic License 2.0). **10,800+ GitHub stars**, **2.5M+ monthly downloads**. Features **tracing** via OpenTelemetry-based instrumentation, **evaluation** using LLMs to benchmark performance, **datasets** for versioned examples, **experiments** for tracking prompt/model/retrieval changes, **playground** for prompt optimization and model comparison, and **prompt management** with version control. Vendor and language agnostic with out-of-the-box support for LlamaIndex, LangChain, Haystack, DSPy, smolagents, and LLM providers including OpenAI, Bedrock, MistralAI, VertexAI, LiteLLM, and Google GenAI. **Runs practically anywhere**: local machine, Jupyter notebook, containerized deployment, or cloud.

- **[TruLens](https://github.com/truera/trulens)**  
  **The most comprehensive open-source evaluation and tracking framework for LLM experiments and RAG pipelines** (Apache-2.0). **3,000+ GitHub stars.** **OpenTelemetry-native**—instrument any app with a decorator, score every step with LLM judges that explain themselves, compare versions, and ship the one that earns it. **Seven purpose-built evaluators for agentic systems**. **Judges are graded against human annotations out of the box**: **95% agent errors caught with Agent GPA on TRAIL/GAIA** (vs 55% baseline). Adopted by **Walmart Global Tech, Cisco, J.P. Morgan Chase, Equinix, VMware by Broadcom, Hitachi Digital Services, Thomson Reuters**.

- **[Langfuse](https://github.com/langfuse/langfuse)**  
  **Open-source LLM engineering platform** (MIT core) with tracing, evaluations, prompt management, and datasets. **35,000+ GitHub stars**. Self-hostable. **Acquired by ClickHouse in January 2026 with commitment to keep it open source**.

- **[Comet Opik](https://github.com/comet-ml/opik)**  
  **Fully-permissive Apache-2.0 rival to Langfuse**. **22,000+ GitHub stars**. Full platform—backend included—free to self-host. Covers AI agent tracing, LLM evaluation, prompt optimization, production monitoring, and **Opik Guardrails**.

- **[DeepEval](https://github.com/confident-ai/deepeval)**  
  **Simple-to-use open-source LLM evaluation framework** (Apache-2.0), similar to Pytest but specialized for unit testing LLM outputs. **The most practical open-source eval framework for CI/CD integration.** Features **large variety of ready-to-use metrics** powered by ANY LLM or local NLP models: G-Eval, Summarization, Answer Relevancy, Faithfulness, Contextual Recall, Contextual Precision, RAGAS, Hallucination, Toxicity, Bias. **Red teaming** for 40+ safety vulnerabilities.

- **[OpenLLMetry (Traceloop)](https://github.com/traceloop/openllmetry)**  
  **Apache-2.0 OpenTelemetry instrumentation for LLM providers, vector DBs, and frameworks**. Emits standard `gen_ai` spans portable to any OTel backend. **The cleanest standards story: no lock-in, pure instrumentation.**

- **[Ragas](https://github.com/vibrantlabsai/ragas)**  
  **The leading open-source RAG evaluation framework** (Apache-2.0). Features **objective metrics** (LLM-based and traditional), **test data generation**, **seamless integrations** with LangChain and major observability tools, and **feedback loops** leveraging production data.

- **[Promptfoo](https://github.com/promptfoo/promptfoo)**  
  **Open-source LLM testing and red-teaming framework** (MIT). **20,000+ GitHub stars.** Listed as one of five tools people actually use for LLM evaluation alongside Braintrust, LangSmith, Inspect, and Ragas.

- **[Inspect](https://github.com/UKGovernmentBEIS/inspect_ai)**  
  **Open-source framework for large language model evaluations from UK AI Safety Institute**. **The most authoritative open-source evaluation framework from a government AI safety body.**

- **[AgentCompass](https://github.com/open-compass/AgentCompass)**  
  **Unified open-source evaluation infrastructure for agents** (Apache-2.0, EMNLP 2026 Demo Track). **30+ public benchmarks and 10+ agent harnesses**. **Composable architecture** decouples Model, Benchmark, Harness, and Environment. **Traceable and reproducible** with trajectory recording, tool calls, and failure analysis.

### Additional Strong Open-Source Options

- **[WhyLogs](https://github.com/whylabs/whylogs)** — Open-source data logging library for AI observability (Apache-2.0). Statistical profiling and drift detection .
- **[Evidently](https://github.com/evidentlyai/evidently)** — Open-source ML and LLM observability (Apache-2.0). Data drift, target drift, and model performance monitoring .
- **[NannyML](https://github.com/NannyML/nannyml)** — Open-source post-deployment model monitoring (Apache-2.0). Performance estimation without ground truth .
- **[Cleanlab](https://github.com/cleanlab/cleanlab)** — Data-centric AI library for label error detection (AGPL-3.0) .
- **[OpenTelemetry GenAI Semantic Conventions](https://github.com/open-telemetry/semantic-conventions-genai)** — Vendor-neutral standard attribute names for model calls, agents, and tool use .
- Community **n8n** workflows for observability alerting and regression detection automation.

**Frameworks for building custom systems**: Combine **Arize Phoenix** for OpenTelemetry-native tracing with **TruLens** for comprehensive evaluation and tracking, **Langfuse** or **Opik** for full-platform observability, **DeepEval** for CI/CD-integrated testing, and **OpenLLMetry** for portable instrumentation—creating a fully self-hosted, enterprise-grade AI observability platform.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- AI observability platforms handling prompts and traces must comply with data protection regulations (GDPR, CCPA, etc.), especially when traces contain PII.
- **"Open source" means different things in this category.** TruLens, DeepEval, Langfuse, Opik, Ragas, Promptfoo, Inspect, and OpenLLMetry are genuinely open source (Apache-2.0/MIT). Arize Phoenix uses Elastic License 2.0 (source-available, not OSI-approved). LangSmith and Braintrust are closed SaaS with open SDKs. **Check the LICENSE file, not the marketing page** .
- **Self-hosting is a hard requirement when prompts or traces carry regulated data.** If they do, the field collapses to Phoenix, TruLens, Langfuse, Opik, and OpenLLMetry. LangSmith and Braintrust cannot self-host on lower tiers .
- **Observability is not evaluation.** Tracing tells you what happened; evaluation tells you whether it was good. Most tools ship both—which makes it easy to buy one and never configure the other. **Tracing alone will not catch quality drift.**
- **OpenTelemetry is the standards bet.** Phoenix, TruLens, Langfuse, Opik, and OpenLLMetry all emit OTel-compatible spans. **Building on OTel now makes switching tools later much easier** .
- **Evaluation judges are themselves LLMs.** Their scores are probabilistic and should be validated against human annotations for high-stakes decisions. TruLens grades its judges against human annotations out of the box—a practice every deployment should follow .
- Self-hosted open-source solutions require proper security hardening, LLM infrastructure (or API keys), and ongoing maintenance. Observability is infrastructure—budget for it accordingly.

---

**Made for ML engineers, platform teams, and developers building transparent AI observability solutions.**  
Let's make AI Observability & Evaluation more open, data-driven, and quality-obsessed.
