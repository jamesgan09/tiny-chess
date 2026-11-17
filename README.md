# Tiny Chess

[![tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/c/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/jamesgan09/tiny-chess/rank.svg)](https://make.fun/c/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/reward.svg)](https://make.fun/c/tiny-chess-01)

A tiny chess engine for the [tiny-chess-01](https://make.fun/c/tiny-chess-01) bounty on make.fun.

`main.py` is a compressed Python engine (LZMA, via the make.fun kit CLI) that fits the 4,096-byte entry limit. It plays through the make.fun env (`MAKEFUN_ENV_URL`): 0x88 board, alpha-beta + quiescence, transposition table, killers, history, null-move pruning, LMR, and futility pruning, with a fixed node budget per move (never a clock), so a replay plays the same moves.

Run it with `MAKEFUN_ENV_URL` set to the env server, e.g. `MAKEFUN_ENV_URL=http://localhost:8080 python3 main.py`.

MIT licensed.
