[![tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/bardah26/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/bardah26/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

# Tiny Chess Engine

A compact chess engine in a single `main.py` (Python 3.13, stdlib only, under 4 KB). Alpha-beta search with quiescence, transposition table, and incremental material + piece-square evaluation. Plays via HTTP against the Make.fun environment.

Bounty: https://make.fun/bounty/tiny-chess-01

## Run

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 main.py
```

The engine reads `MAKEFUN_ENV_URL`, `MAKEFUN_PROMPT_FILE`, and `MAKEFUN_TRIAL_SEED` from the environment. It is fully deterministic: fixed node budget per move, no wall-clock use, no randomness.
