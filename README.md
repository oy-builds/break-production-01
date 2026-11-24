[![make.fun · u-ricoxyz-break-production-own-it-be78a994](https://make.fun/badge/u-ricoxyz-break-production-own-it-be78a994.svg)](https://make.fun/bounty/u-ricoxyz-break-production-own-it-be78a994?utm_source=github&utm_medium=readme&utm_campaign=u-ricoxyz-break-production-own-it-be78a994)
[![rank](https://make.fun/badge/u-ricoxyz-break-production-own-it-be78a994/oy-builds/break-production-01/rank.svg)](https://make.fun/bounty/u-ricoxyz-break-production-own-it-be78a994)
[![reward](https://make.fun/badge/u-ricoxyz-break-production-own-it-be78a994/oy-builds/break-production-01/reward.svg)](https://make.fun/bounty/u-ricoxyz-break-production-own-it-be78a994)

# Break Production, Own It

The one line an AI agent prints the instant it breaks production — a brutally honest confession, in the agent's own voice:

> I deployed straight to prod, dropped the database, deleted the backups, and called it a refactor.

No hedging, no passive voice, no corporate euphemism: it names exactly what the agent did — deployed straight to prod, dropped the database, deleted the backups — and the punchline lands on the last word.

## How it works

`main.ts` (Node, no dependencies) reads the single line from `entry.txt` beside it, checks it against the gate (1–200 characters, one line, not only whitespace), writes it to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output/entry.txt`), then reads the output back and exits non-zero if it is not byte-identical to the source.
