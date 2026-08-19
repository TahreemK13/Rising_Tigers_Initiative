# /artifacts/

Everything that argues something belongs here — one folder per piece, whether it's mine or a contributor's.

## Adding a piece

```
/artifacts/<slug>/
├── index.html (or index.md)
└── (any assets the piece needs)
```

Give each piece simple front matter at the top of its source file:

```yaml
---
title:
author:
date:
cites: []  # library claim IDs this piece draws on
---
```

`cites` is what keeps provenance attached to the piece even once it's not just one person writing these — see `docs/reference/sources-schema.md` for what a claim ID looks like.

Reference `/library/` by absolute path (`/library/sources.json`), never relative — pieces at different folder depths would each need a different number of `../`, and it's an easy thing for a contributor to get wrong.
