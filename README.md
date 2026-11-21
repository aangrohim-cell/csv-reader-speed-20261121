# csv-reader-speed 20261121

[![make.fun · csv-reader-speed-01-run-20261121](https://make.fun/badge/csv-reader-speed-01-run-20261121.svg)](https://make.fun/bounty/csv-reader-speed-01-run-20261121)
[![rank](https://make.fun/badge/csv-reader-speed-01-run-20261121/aangrohim-cell/csv-reader-speed-20261121/rank.svg)](https://make.fun/bounty/csv-reader-speed-01-run-20261121/leaderboard)
[![reward](https://make.fun/badge/csv-reader-speed-01-run-20261121/aangrohim-cell/csv-reader-speed-20261121/reward.svg)](https://make.fun/bounty/csv-reader-speed-01-run-20261121)

Entry for the make.fun bounty **Read broken CSV files faster, 21 November 2026**.

## What it does

- `main.ts` reads `/input/cases.json`, runs `solve.js` for each case, and writes `/output/answers.json`.
- `solve.js` implements `run(input)` and returns the same answer shape expected by the scorer for each input case.
- The implementation is based on the house csv-reader baseline shipped in the kit, kept correct while packaged as a clean repository entry.

## Layout

- `main.ts` — entrypoint run by the harness (`node /bot/main.ts`)
- `solve.js` — CSV reader `run(input)` implementation
- `vendor/csv-reader/` — vendored csv-reader package used by `solve.js`
- `LICENSE` — MIT

## Local notes

The official dev/practice grading flow is provided by the competition kit:

```bash
node cli/makefun.mjs grade-local --kit . --bot <repository> --driver docker
```

This repo is structured so it can be submitted as a make.fun GitHub entry.
