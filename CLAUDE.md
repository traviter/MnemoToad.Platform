# MnemoToad.Platform — Project Conventions

## Purpose

This repo holds cross-cutting platform documentation that doesn't belong to any single service repo — architecture references, schema diagrams, API-interaction diagrams, design decisions that span `MnemoToad.Knowledge`, `MnemoToad.Learning`, and future services (a Gateway, frontends). It is documentation-only for now: no application code, no build, no tests.

Sibling repos: [traviter/MnemoToad.Knowledge](https://github.com/traviter/MnemoToad.Knowledge) (the graph/"dictionary of things"), [traviter/MnemoToad.Learning](https://github.com/traviter/MnemoToad.Learning) (Leitner-box spaced repetition). Each service still owns its own conventions in its own `CLAUDE.md` — this repo doesn't restate those, only the decisions that cross service boundaries.

## Contents

- `docs/architecture.html` — the platform architecture & schema reference (ER diagram, property-path DSL, API interaction diagrams, build sequencing). Deliberately a standalone HTML file, not Markdown — the user wants room to grow it into a more advanced navigable document (e.g. embedding a third-party schema-diagram renderer) without being constrained by what GitHub's Markdown preview can render. Regenerate/update it when the underlying design changes materially rather than letting it drift out of sync with the actual plan.

## Commit conventions

Same as the other MnemoToad repos: no story numbers, matter-of-fact commit messages (list what changed, skip rationale/motivation prose).
