# token-radar-01

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/simpson007/token-radar-01/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/simpson007/token-radar-01/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

Token Radar ranks the pre-token protocols in DefiLlama's sealed snapshot by implied value and shows a reader how to farm each one. The board covers all 40 watchlist protocols plus the 160 largest pre-token protocols below the $50M floor, 200 rows in all. Each protocol is priced off its own category's live-token comparables — the median market-cap-to-TVL ratio of the live-token protocols in its category — adjusted by seven-day TVL growth and by how long it has run with no token. The dashboard is a static page with a sortable, filterable board, a detail view for every protocol with its model breakdown and farm plan, and a separate live-token view for the protocols that already trade.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input <path to snapshot.json>
```

`main.ts` (Node 22, standard library only) reads the snapshot, writes `board.json`, `data.js`, `dashboard/` and `screenshots/` to the output directory, and writes `dossier.json` with the vendored make.fun library (`vendor/makefun-board.ts`, copied from the competition kit). Open `out/dashboard/index.html` in a browser to use the radar.

---

<sub>Entered on [make.fun](https://make.fun/?ref=ngqr1ydj&utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards</sub>
