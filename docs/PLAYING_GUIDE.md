# REVERSI - BASIC MASTER LEVEL2II

## Playing Guide

### Computer strength

| Key | Level | Search depth | Maximum thinking time |
|---|---|---:|---:|
| `1` | BEGINNER | 2 | 5 sec |
| `2` | INTERMEDIATE | 3 | 10 sec |
| `3` | ADVANCED | 4 | 20 sec |

### FIRST / SECOND

| Key | Selection | YOU | COM |
|---|---|---|---|
| `1` | FIRST | BLACK | WHITE |
| `2` | SECOND | WHITE | BLACK |

BLACK moves first.

### Board symbols

- `●` : BLACK
- `○` : WHITE
- `・` : legal move
- blinking cursor : currently selected legal move

### Cursor controls

```text
     I
   J + K
     M
```

- `I` : move to the next legal position, preferring the upward direction
- `J` : move to the next legal position, preferring the left direction
- `K` : move to the next legal position, preferring the right direction
- `M` : move to the next legal position, preferring the downward direction
- `RETURN` : place a disc on the selected square
- `Q` : quit

### COM turn

While the COM is thinking, the right-side panel displays the elapsed time and the maximum thinking time.

### PASS

If the current player has no legal move but the opponent does, the turn is passed.

### Game over

The game ends when neither player has a legal move.
The right-side panel displays `YOU WIN`, `COM WINS`, or `DRAW`, together with the final disc counts.

- `R` : RESTART
- `Q` : QUIT
