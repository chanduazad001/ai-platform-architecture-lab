# ai-platform-architecture-lab

Public MkDocs site at `/ai-platform-architecture-lab/`. Group rules in `../CLAUDE.md` apply. This lab is the newest and still being built.

## Purpose
Architecture of AI platforms from the infrastructure and platform-engineering side — the bridge to an AI Infrastructure Architect role.

## Content model
- Platform reference architectures: LLM gateway/routing, RAG pipelines, vector stores, evaluation, guardrails, observability (tokens, latency, cost).
- AI infrastructure: GPU scheduling on Kubernetes, model serving, capacity and cost modelling.
- AI security: prompt injection, data leakage, tool/agent permissions, supply chain of models.
- Each topic ends with an ADR and an explicit trade-off table.

## Rules
- Model names, prices and capabilities change fast: date every comparison ("as of YYYY-MM") and cite the source.
- Prefer patterns that are vendor-neutral; name vendors as examples, not as the architecture.
- Private builds in `../../private/` (e.g., the knowledge platform or LLM debate platform) may be written up here only as sanitised case studies — never copy their config, hostnames or IPs.

## Build
`mkdocs build --strict` must pass. Update `nav:` in `mkdocs.yml` for new pages.
