# PromptWeave

> **The Git for Prompts** — Manage, test, and deploy AI prompts across multiple models.

PromptWeave is an open-source **AI Prompt Engineering Platform** that helps development teams manage the full lifecycle of AI prompts: authoring, versioning, testing, evaluation, and deployment.

## Why PromptWeave?

As LLMs multiply (GPT, Claude, Gemini, DeepSeek, Qwen...), teams face a new challenge: managing hundreds of prompts across multiple models, environments, and experiments.

PromptWeave solves this with:

- **Version Control** — local/test/prod three-stage versioning (like Git branches for prompts)
- **MetaPrompt** — Define once, generate N variants for different models/platforms/experiments
- **Multi-Environment Sync** — Pull/Push with pluggable adapters to sync with any business system
- **Playground** — Test prompts against multiple models side-by-side *(v1.1)*
- **Dataset & Evaluation** — Batch testing with scoring and regression detection *(v1.2)*
- **Prompt Workflow** — DAG-based prompt chain orchestration *(v2.0)*

## Quick Start

```bash
docker compose up
```

> Coming soon. PromptWeave is under active development.

## Tech Stack

| Layer | Technology |
|-------|------------|
| Backend | NestJS 11 + Fastify + TypeScript |
| ORM | Prisma (PostgreSQL) |
| Validation | Zod v3 + nestjs-zod |
| Frontend | React 19 + Ant Design 6 |
| Testing | Vitest |
| Package Manager | pnpm |

## Roadmap

| Version | Features | Status |
|---------|----------|--------|
| v1.0 | Prompt/Snippet/Provider CRUD + Versioning + Sync + MetaPrompt | In Progress |
| v1.1 | Playground + Dataset + LCA Context Engine | Planned |
| v1.2 | Batch Evaluation + A/B Comparison + Regression Testing | Planned |
| v2.0 | Prompt Workflow (DAG orchestration, inspired by n8n) | Planned |

## Unique Features

### MetaPrompt Batch Variants

Define a base prompt and generate variants for every model/platform/experiment combination with one click. No competitor offers this.

### LCA Smart Context (v1.1)

Powered by [llm-context-attention](https://github.com/me-tool/llm-context-attention) — topic-aware context routing that saves ~50% tokens in multi-turn Playground conversations.

### SyncAdapter Pattern

Pluggable adapters to sync prompt configurations with any business system via Pull/Push. Not locked into any specific SDK.

## Contributing

Contributions are welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## License

[MIT](LICENSE)
