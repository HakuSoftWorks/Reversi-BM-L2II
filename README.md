# REVERSI - BASIC MASTER LEVEL2II

**REVERSI - BASIC MASTER LEVEL2II** is a Reversi game for the Hitachi BASIC MASTER LEVEL2II (MB-6881).
It is written for the Hitachi HD46800 8-bit MPU, which is instruction-set compatible with the Motorola MC6800, and runs in a 16KB RAM environment.

**Version 1.0 — Initial Release**

Japanese documentation: [README-J.md](README-J.md)

## Features

- 8×8 Reversi
- FIRST / SECOND selection
- 3 computer strength levels
- legal-move markers and blinking cursor
- `I / J / K / M` cursor movement
- turn, score, and computer thinking-time display
- Negamax search with alpha-beta pruning
- positional evaluation and mobility
- exact endgame search
- PASS handling

## Actual Hardware Demo

REVERSI v1.0 running on an actual Hitachi BASIC MASTER LEVEL2II (MB-6881).

https://youtu.be/aiN6JqGPsug

## Screenshots

### Human turn
Legal moves are shown with `・`, and the selected legal move is indicated by the blinking cursor.

![REVERSI - Human turn](images/reversi_your_turn.png)

### Computer thinking
During the computer turn, the elapsed and maximum thinking time are displayed.

![REVERSI - Computer thinking](images/reversi_com_thinking.png)

## Target

- Hitachi BASIC MASTER LEVEL2II (MB-6881)
- Hitachi HD46800, MC6800-compatible
- 16KB RAM
- load / start address: `$1000`
- character VRAM: `$0100-$03FF` (32 × 24)

## Run

`bin/` contains:

- `reversi6800_BM_L2II_v1.0.bin` — raw binary
- `reversi6800_BM_L2II_v1.0.s19` — Motorola S-record

For the raw BIN, load it at `$1000` and start execution from `$1000`.
The S-record contains its load addresses and uses `$1000` as the execution entry.

See [docs/PLAYING_GUIDE.md](docs/PLAYING_GUIDE.md) for the playing guide.

## Copyright

Copyright (C) 2026 Haku Soft Works. All rights reserved.

See [COPYRIGHT.txt](COPYRIGHT.txt) and [NOTICE.md](NOTICE.md).
