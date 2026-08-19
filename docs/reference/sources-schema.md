# Sources schema

One entry per **claim**, not per document — a single article can back several claims, and a single claim can be backed by several articles.

| Field | Required | Notes |
|---|---|---|
| `id` | yes | Stable identifier — artifacts cite this |
| `claim` | yes | The specific assertion, one sentence |
| `figure_type` | yes | `count` \| `range` \| `estimate` \| `projection` \| `disputed` |
| `value` | yes | The number, range, or figure itself |
| `source` | yes | Where it came from |
| `checked` | yes | Date last verified |
| `caveat` | required unless `figure_type` is `count` | What's soft about this figure and why |
| `archive_url` | required if `figure_type` is `disputed` | Archived copy — disputed pages get edited |

`library/sources.md` is the human-editable source of truth. Machine-readable exports (`sources.csv`, `datapackage.json`) are meant to be generated from it, not maintained by hand — that generation pipeline is still to be built, once there's a real release to cut.
