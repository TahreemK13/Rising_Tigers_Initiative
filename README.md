# Rising Tigers Initiative

A public resource hub by the Rising Tigers Initiative and its sources.

**Live at:** [risingtigers.tahreemkarim.xyz](https://risingtigers.tahreemkarim.xyz)

Maintained by [Tahreem Karim](https://portfolio.tahreemkarim.xyz). Everything here is free and
linked to a primary source. Corrections welcome!

Welcome to the Rising Tigers repo! Below is how the folders are broken down, plus the fonts,
palette, and archival ideas that shaped how everything here is built — helpful if you're
forking, contributing, or just curious how the pieces fit together.

## Why

"Source?" should be an easy answer, and because a link in in public rots loudly, where anyone can catch it.

## Structure

| Path | What it holds |
|---|---|
| `/` | Hub — links to everything below, plus out to [portfolio](https://portfolio.tahreemkarim.xyz), [garden](https://garden.tahreemkarim.xyz), and [free resources](https://tahreemkarim.xyz) |
| `/activism` | The flagship artifact — Sudan/Congo/Palestine displacement, Bengal tiger/deforestation/pollution |
| `/artifacts/<slug>/` | Every other piece — articles, dashboards, projects, mine or a contributor's |
| `/library/` | The sourced claim collection everything above cites into — forkable, correctable, meant to grow into its own resource over time |
| `/docs/` | How this repo is organized and how to contribute |

## The distinction between the library and an 'artifact'

If it argues something, it's an artifact. If it substantiates an argument, it's the library. Full reasoning in [`docs/explanation/documentation-standards.md`](docs/explanation/documentation-standards.md).

## What's *not* here

- **Book reviews** → those live in [the library](https://garden.tahreemkarim.xyz/library). Personal, not reference.
- **Half-formed thinking** → [the garden](https://garden.tahreemkarim.xyz). Nothing there is finished on purpose.
- **My own papers and code** → [portfolio](https://portfolio.tahreemkarim.xyz).

## Resources

A few things worth knowing if you're reading the code, not just the site:

**Typography** — [Instrument Serif](https://fonts.google.com/specimen/Instrument+Serif) for
display headings, [Public Sans](https://fonts.google.com/specimen/Public+Sans) for body text,
and [DM Mono](https://fonts.google.com/specimen/DM+Mono) for figures and metadata, all pulled
from Google Fonts. No build step — just a `<link>` in each page's `<head>`.

**Palette** — each page defines its colors as CSS custom properties (`--morado`, `--rosa`,
`--turquesa`, `--verde`, `--marigold`, `--candle`, `--bone`, `--ink`, `--night`), with separate
day/night variants for a few of them. Changing the palette anywhere means editing those
variables at the top of the page's `<style>` block, not hunting for hex codes in the markup.

**No JS frameworks** — every page here is hand-written HTML/CSS, no React, no build pipeline.
That's deliberate: guerrilla-archiving practice (below) means a page should stay readable and
forkable without `npm install`.

**The archival traditions behind the structure** — the split between `/artifacts/` (things with
a point of view, meant to be read) and `/library/` (sourced claims, meant to be queried and
cited into) borrows from four older traditions: archival *respect des fonds* (provenance as a
required field, not a footnote), GNU/Debian flat-text root files (`README`, `LICENSE`,
`CITATION.cff` — orientation without JavaScript), zine colophons (crediting exactly how a thing
was made), and guerrilla-archiving practice (assume your own host disappears; forking is a
feature, not an edge case). The full reasoning is in
[`docs/explanation/documentation-standards.md`](docs/explanation/documentation-standards.md).

## Contributing

**Open an issue** if a link is dead, a figure is stale, or something obvious is missing. If you're
adding an entry, include the primary source *and the date you checked it*.

## License

Code: MIT (see `LICENSE`). Written content and the library's data: CC BY 4.0 (see `LICENSE-DATA`).
Underlying data belongs to whoever produced it; follow each source's own terms.

## Citing this work

See `CITATION.cff`.
