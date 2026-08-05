# PARSEC

**P**ipelines · **A**gents · **R**etrieval · **S**emantic **E**ngineering of **C**ontext

*An open, forkable toolkit for grounding AI agents in real astronomy.*

> ⚠️ **Placeholder scaffold — early days.** The structure and the contribution
> model are here first; the tools grow with the community. Expect this to change.

---

## The idea

AI models are fluent and, on the specifics of *your* science, often quietly wrong.
**Grounding** fixes that — put the right facts, data, and methods in front of the
model at answer time, from a source *you* curate and can read.

PARSEC will be a collection of small, dependency-light **MCP tools and patterns**
that do exactly that for astronomy: retrieval over your own knowledge base, survey /
catalog access, pipeline and reproduction helpers — each readable in a sitting.

**Science gets better when we work together.** Fork it, add the tool your group
needs, send it back. No API keys, no vendor lock. That's the whole point.

## Start here

Want to *see* grounding change a real answer first? The hands-on companion is RAG
over a knowledge base in ~90 lines of stdlib Python, no account, no cloud:

**→ [westoverlabs/parsec-rag-demo](https://github.com/westoverlabs/parsec-rag-demo)**

That's the on-ramp. This repo is where the reusable tools will live and grow.

## Contributing

Read [`AGENTS.md`](./AGENTS.md) — the shape and standards every tool follows
(applies to AI-agent contributors too). Then fork, add your piece, open a PR
describing what you verified by actually running it. Nothing is too small.

## License

MIT — see [`LICENSE`](./LICENSE). Built by Westover Labs for the LSST / Rubin
community and anyone doing science with agents.
