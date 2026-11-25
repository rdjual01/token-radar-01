# Launch Radar — token-radar-01

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/rdjual01/token-radar-01/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/rdjual01/token-radar-01/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

A token launch radar that prices pre-token protocols the way the market prices their
category: each protocol's implied value is its TVL times its category's live-token
median market-cap-per-TVL, shrunk toward the market-wide median and adjusted for
seven-day growth, age with no token, and chain breadth. The board covers the whole
40-protocol watchlist plus 260 early pre-token protocols below the floor, each with a
seven-step farm plan, and the dashboard shows the board, a detail view per protocol,
filters, the live-token comps, and the model stated in full.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input ../input/snapshot.json
```

`main.ts` (Node 22, standard library only) reads the sealed snapshot, writes
`board.json`, `data.js` and `dossier.json` to the output directory, and copies
`dashboard/` and `screenshots/` there. Open `out/dashboard/index.html` in a browser;
it renders with no network.

---

<sub>Entered on [make.fun](https://make.fun/?ref=rdjual01&utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards</sub>
