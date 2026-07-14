# llm-wiki-starter

A ready-made skeleton for an AI agent's **layered long-term memory**: rules ·
memory · wiki · skills. It extends the [Karpathy LLM-wiki method](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)
— the wiki is one layer of four, not the whole system.

An AI coding agent starts every session from scratch and forgets. Dumping
everything into one file breaks within a week: it bloats, facts duplicate, copies
drift. This repo is a **layered** storage system where each layer has one role —
clone it, keep the layers your scale needs, fill them with your own content.

> **🇷🇺 This project is Russian-first.** The full documentation, the scale ladder
> that tells you which layers you actually need, and the method guides all live in
> **[README.ru.md](README.ru.md)** — start there.

License: [MIT](LICENSE).
