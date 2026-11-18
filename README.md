# Tiny Chess

A chess engine in 4,096 bytes of Python, built for [tiny-chess-01](https://make.fun/bounty/tiny-chess-01) on make.fun.

[![tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/contact-nathanealphi/tiny-chess-20261119/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/contact-nathanealphi/tiny-chess-20261119/reward.svg)](https://make.fun/bounty/tiny-chess-01)

0x88 board, alpha-beta with iterative deepening on a fixed node budget,
transposition table, killers, history ordering, null-move pruning, late-move
reductions, quiescence with check evasions, and a tapered piece-square
evaluation with pawn structure. `main.py` is the whole engine, packed from
`engine.py` with the kit's `makefun compress`; it plays the house gauntlet
through the env at `MAKEFUN_ENV_URL`, deterministically: fixed nodes, no clock.
