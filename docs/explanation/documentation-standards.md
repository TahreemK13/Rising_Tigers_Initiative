# Why this repo is organized the way it is

## The archival traditions behind the schema

There isn't a codified body of "how activists should document sourced claims" to borrow from, so this project leans on four older traditions instead, each solving a piece of the problem:

**Archival *respect des fonds*** — the principle that a record's origin and chain of custody matter as much as its content. It's why `library/sources.md` treats provenance as a required field per claim rather than a footnote you could drop, and why the schema is one entry per *claim*, not per document — a claim's history should be traceable independent of whatever else its source document said.

**GNU/Debian flat-text root files** — `README`, `LICENSE`, `CITATION.cff`, all readable in thirty seconds without a rendered website. Orientation shouldn't require JavaScript.

**Zine colophons** — a tradition of crediting exactly how a thing was made and explicitly granting permission to copy it. The split MIT/CC BY licensing and the contributor docs are this project's colophon.

**Guerrilla-archiving practice** — assume your own host disappears. It's why an offline-capable bundle is planned for the activism page, and why forking is treated as a feature of this repo, not an edge case.

## Artifacts vs. the library

The word "artifact" gets used two ways in research and journalism, and both are legitimate — a finished piece meant to be read start to finish, or any citable, versioned output, including a dataset. This repo needs to pick one sense, because `/artifacts/` and `/library/` sit side by side, and a contributor needs to know instantly which their work belongs in.

The rule: **if it argues something, it's an artifact. If it substantiates an argument, it's the library.**

The activism page has a point of view — it's curated, framed, and sequenced on purpose. The library deliberately doesn't argue anything; a skeptical reader should be able to check a claim without having to trust the framing around it at all. That's not the library being a smaller or plainer artifact — it's a structurally different object. Artifacts are meant to be read. The library is meant to be queried and cited into.

Practically: `/library/` is a sibling of `/artifacts/`, not a child of it. If something would put a schema document or a contributor code of conduct in the same listing as a piece meant to be experienced end-to-end, it's drifted from this rule.
