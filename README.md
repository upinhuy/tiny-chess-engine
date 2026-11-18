# tiny-chess-engine

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/upinhuy/tiny-chess-engine/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/upinhuy/tiny-chess-engine/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 3,208 bytes of Python. 0x88 board, negamax alpha-beta
with quiescence search, a transposition table, killer moves and a history
heuristic for ordering, delta and futility pruning, check extensions, and a
separate endgame king table. It searches a fixed budget of 150,000 nodes per
move, so it is fully deterministic: the same position always yields the same
move. Practice trial on the make.fun gauntlet: 4 wins, 2 losses, Elo 1,451.

## Run it

`main.py` is the entrypoint, packed from a readable source with the
competition's LZMA packer. It speaks the make.fun env protocol over HTTP:

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8123 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=hv9zk8y5&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
