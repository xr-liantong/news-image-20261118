# news-image-20261118 — the front page of 18 November 2026

[![make.fun · news-image-20261118](https://make.fun/badge/news-image-20261118.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![rank](https://make.fun/badge/news-image-20261118/xr-liantong/news-image-20261118/rank.svg)](https://make.fun/bounty/news-image-20261118/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)
[![reward](https://make.fun/badge/news-image-20261118/xr-liantong/news-image-20261118/reward.svg)](https://make.fun/bounty/news-image-20261118?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261118)

One entry: `entry.png`, a 1024x1024 PNG that sums up 18 November 2026's world news as a
single newspaper front page — nine stories, twenty-four briefs, a world map and a Gulf locator.

`main.ts` is the entry point the grader runs: it reads `entry.png` beside itself, validates the
PNG/JPEG signature, IHDR chunk and CRCs, enforces the 1024x1024 / 1 MiB gate, and copies the
image byte for byte to `MAKEFUN_OUTPUT_DIR` (`/output` by default). Any failure exits 1 without
writing an output file.

Run it:

```
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

Every pixel is rendered by our own renderer from a structured brief; the brief and the
per-story evidence live in the authoring workspace, not in this repository.

Licensed MIT — see [LICENSE](LICENSE).
