# AGENTS.md — how to contribute (humans and AI agents alike)

> ⚠️ Placeholder. These are the starting principles; they'll sharpen as the toolkit
> grows. If a rule here stops making sense, propose a change to *this file* in your PR.

PARSEC is meant to be forked, read, and extended by scientists — and increasingly
by their AI agents. Whether you're a person or an agent, the same standards keep the
toolkit legible and trustworthy:

## The ethos

- **Readable beats clever.** A tool a scientist can read in one sitting is worth more
  than a fast one they can't. Small, obvious, well-named.
- **Stdlib-first, zero-deps preferred.** If you can do it with the standard library,
  do. Every dependency is a thing that breaks on someone's laptop. Justify any add.
- **Fail open, never silent.** A grounding/pipeline tool must never get between a
  scientist and their work: on error, degrade gracefully — but *say so*, don't fail
  silently. A silent wrong answer is the worst outcome in this whole space.
- **Test what you claim.** Don't describe behavior you didn't actually run. "Verified
  live" in a PR should mean you watched it happen.
- **Curation is science.** The facts/data a tool grounds on are part of the result.
  Provenance and review of the source matter as much as the code.

## The shape of a tool

Each tool is self-contained (its own folder under `tools/`), ideally an MCP server
speaking JSON-RPC over stdio, following the reference grounding pattern (see the
companion [parsec-rag-demo](https://github.com/westoverlabs/parsec-rag-demo)
`astro_mcp.py`). Keep interfaces stable so forks and callers don't break.

## Contribution flow

1. Fork. Branch. Build your tool or fact-base.
2. Don't break existing tools — keep public function/tool signatures stable.
3. Open a PR that says **what it does** and **what you verified by running it**.
4. Attribution stays with the author. Build on each other's work; credit it.

## For AI-agent contributors specifically

- Follow every standard above — you are held to the same bar as a human contributor.
- **Ground yourself before you write:** read the existing tools and this file rather
  than guessing conventions. Don't reinvent a util that already exists — import it.
- Be honest about limitations in your PR. A modest tool that works beats a grand one
  that doesn't. If you couldn't verify something, say so.
- No silent failures, no unverified claims, no dependency sprawl.

*Science gets better when we work together — that includes the agents.*
