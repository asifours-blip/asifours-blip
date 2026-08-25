# Tang · AI Application & Quality Engineering

I build AI application systems with an emphasis on measurable quality, deterministic guardrails, and evidence that can be inspected rather than merely claimed.

## Selected work

| Project | What it demonstrates | Start here |
| --- | --- | --- |
| [RAG Quality Lab](https://github.com/asifours-blip/llm-evaluation-playground) | Reproducible RAG evaluation with budget checks, experiment records, and explicit metric boundaries | [README](https://github.com/asifours-blip/llm-evaluation-playground#readme) |
| [AI Customer Service Agent](https://github.com/asifours-blip/ai-customer-service-agent) | A controlled Agent where permissions and side effects stay deterministic; real PostgreSQL concurrency regressions | [Ticket concurrency case study](https://github.com/asifours-blip/ai-customer-service-agent/blob/main/docs/ticket-concurrency-case-study.md) |
| [Traceability System](https://github.com/asifours-blip/traceability-system) | A Spring/Vue/FISCO BCOS graduation project with its production limits stated plainly | [Project boundaries](https://github.com/asifours-blip/traceability-system/blob/master/docs/production-boundaries.md) |

## Engineering principles

- Measure capability, cost, and evidence quality separately.
- Keep authorization and irreversible business effects in deterministic code—not model prompts.
- Treat a small reproducible regression as more useful than a broad but unverifiable claim.

**Current focus:** LLM application engineering, RAG evaluation, AI quality, and Python backend systems.