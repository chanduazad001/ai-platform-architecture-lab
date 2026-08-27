# AI Platform Architecture Lab

AI platform architecture and AI system design — documented as deliberate
architecture practice: designs, constraints, trade-offs, and the reasoning
behind decisions for RAG pipelines, model serving, agentic systems, and AI
infrastructure.

**Published site:** https://chanduazad001.github.io/ai-platform-architecture-lab/

Part of a wider set of labs linked from
[chanduazad001.github.io](https://chanduazad001.github.io/), including
[Solution Architecture Lab](https://chanduazad001.github.io/solution-architecture-lab/)
and
[Cybersecurity Architecture Lab](https://chanduazad001.github.io/cybersecurity-architecture-lab/).

## Structure

- **AI Architecture** — end-to-end AI platform case studies, following the
  same Overview → Architecture → Data Flow → Security → Availability →
  Decisions discipline used across the other labs.
- **AI System Design** — the reusable system-design theory behind AI
  platform decisions: scaling inference, retrieval pipelines, evaluation,
  and observability for AI workloads.

Diagrams are written as [Mermaid](https://mermaid.js.org/) inline in the
Markdown, so they stay version-controlled alongside the text.

## Local development

```bash
python -m venv .venv
.venv\Scripts\activate      # Windows
source .venv/bin/activate   # macOS/Linux

pip install -r requirements.txt

mkdocs serve
```

Then open http://127.0.0.1:8000.

## Publishing

Pushes to `master` that touch `docs/`, `mkdocs.yml`, or `requirements.txt`
trigger `.github/workflows/docs.yml`, which builds the site with
`mkdocs build --strict` and deploys it to GitHub Pages.

## License

See [LICENSE](LICENSE).
