# Tic Tac Shuffle

A nested tic-tac-toe game with energy-powered buffs. A 3x3 big board holds nine small 3x3 boards, and the game keeps shuffling which small board you play in.

## How to play

**Rounds**
- The game picks a glowing small board at random.
- X plays one move there, then O replies in the same board. That is one round.
- After each round the game jumps to another undecided board at random, and X starts again.
- If X's move wins or fills the board, the round ends immediately.

**Boards**
- Three in a row in a small board claims that cell of the big board.
- A full small board with no winner is a **TIE** board. It is skipped, but it can be claimed with the Claim buff.

**Winning**
- **SUPER BIG WIN:** claim three big cells in a row, at any time.
- **BIG WIN:** every board is decided first and you hold more big cells.
- If both players hold the same number of big cells, the game is a draw.

## Energy (EP) and buffs

- Both players start with 1 EP and gain 1 EP at the end of every round (max 10).
- You may use **one buff per round**, before your move.
- Both players can use buffs, including the CPU.

| Buff | Cost | Effect |
|------|------|--------|
| Convert | 4 EP | Flip one enemy mark in the glowing board into yours. |
| Redirect | 2 EP | Choose which board the next round is played in. |
| Claim | 10 EP | The ultimate move. Claim a TIE board's big cell for yourself. |

## Modes

- **vs CPU** with three levels: Easy, Normal, Hard. You play X and the CPU plays O. The CPU uses buffs more often on higher levels.
- **2 Players** on the same device, taking turns.

## Run it

Open `index.html` in a browser. No build step, no dependencies. The pixel font loads from Google Fonts, and the game falls back to a monospace font if it is offline.
