# llm-wiki-starter

**🇷🇺 Русская версия (основная): [README.ru.md](README.ru.md)**

A ready-made skeleton for an AI agent's long-term memory and knowledge base. It
extends the [Karpathy LLM-wiki method](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)
— the wiki is one layer of four, not the whole system.

An AI coding agent starts every session from scratch — it forgets. The naive fix
(dump everything into one file) breaks within a week: the file bloats, facts
duplicate, copies drift apart. This repo is the path already walked for you: a
**layered** storage system where each layer has one role.

Clone it, keep the layers your scale actually needs, fill them with your own content.

## The four layers

| Layer | What it holds | Lives in |
|---|---|---|
| **Rules** | how the agent should behave | [`CLAUDE.md`](CLAUDE.md) |
| **Project memory** | pointed facts & feedback, one fact per file | [`projects/demo-project/memory/`](projects/demo-project/memory/) |
| **Knowledge base (wiki)** | portable, cross-linked knowledge | [`wiki/`](wiki/) |
| **Skills** | reusable, shareable methods | [`share/`](share/) |

## Not sure you need this?

If you run one small project, a single notes file is enough. The layers start to
pay off once you have **several** projects and knowledge flows between them. The
"scale ladder" in [README.ru.md](README.ru.md) helps you find your rung.

## What's inside

- [`CLAUDE.md`](CLAUDE.md) — the rules layer (a de-personalized example)
- [`templates/`](templates/) — blank forms for memory files and wiki pages
- [`projects/demo-project/memory/`](projects/demo-project/memory/) — a demo project's memory (index + one fact)
- [`wiki/`](wiki/) — a demo knowledge base with cross-links
- [`share/`](share/) — two reference methods: [storage architecture](share/storage-architecture.md) and the [capability tree](share/capability-tree.md)

The substantial content is in Russian; an English translation of the `share/`
methods is planned separately. License: [MIT](LICENSE).
