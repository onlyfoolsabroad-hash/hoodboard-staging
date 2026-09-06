# HOOD BOARD — compiled deployment artifact

Compiled output only. Source lives in a private repository and is not mirrored here.

| Path | What |
|---|---|
| `/` | HOOD BOARD — the machine world on live Robinhood Chain data (2026-09-06) |
| `/?v1` | the previous Board, served from the same build |
| `/v1/` | frozen copy of the previous production artifact — the rollback |
| `/preview/` | same build as the root; kept so preview links keep working |

Data mode: `mainnet`. The Board reads `live/board.json`, published by the data engine on a schedule; the page shows
its age and block. A missing or day-old payload is an explicit unavailable state — fixtures are never substituted.
The frozen `/v1/` build is fixture mode and says so on screen.
