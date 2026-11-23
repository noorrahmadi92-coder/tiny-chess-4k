# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/noorrahmadi92-coder/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/noorrahmadi92-coder/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A tiny chess engine in 4 KB of Python: 0x88 board, negamax with alpha-beta, iterative deepening on a fixed node budget (never a clock, so replays match), quiescence, transposition table, killers and history ordering, null-move pruning, LMR, and a tapered eval with piece-square terms and pawn structure. It plays the make.fun tiny-chess-01 gauntlet through the env HTTP API.

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 main.py
```

## Verified

- Perft 20/20 correct (including Kiwipete and position 6), mate-in-1 and win-queen tactics found, deterministic, 60-move self-play clean.
- Packed with `makefun compress` from the readable source (`final.py`, kept beside the entry); the entry is 3,229 bytes, under the 4,096-byte cap.

---

<sub>Entered on [make.fun](https://make.fun/?ref=ch0mnr4w&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
