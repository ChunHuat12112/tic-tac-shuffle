# Tic Tac Shuffle

Tic-tac-toe inside tic-tac-toe, with a shuffling board, power-ups and two ways to win.

A 3x3 big board holds nine small 3x3 boards. The game decides which small board you play in, and win small boards to claim big cells.

## How to play

### A round
1. The game picks a glowing small board at random.
2. X plays one move there, then O replies in the same board.
3. The game jumps to another random board, and X starts the next round.

If a move wins or fills the small board, the round ends immediately.

### Claiming big cells
- Get three in a row in a small board to claim that big cell.
- A full small board with no winner shows **TIE**. It stays unclaimed and can be taken with the Claim buff.

### Two ways to win
| Win | How |
| --- | --- |
| **SUPER BIG WIN** | Claim three big cells in a row, at any time. |
| **BIG WIN** | Every board is decided first, and you hold more big cells. |

If the big cells are tied when every board is decided, the game is a draw.

## EP and buffs
- Both players start with 1 EP and gain 1 EP at the end of every round (max 5).
- Each player can use **one buff per round**, before their move.
- Buffs work for both players, and the CPU uses them too.

| Buff | Cost | Effect |
| --- | --- | --- |
| **Convert** | 2 EP | Flip one enemy mark in the glowing board into yours. Only usable while you are behind in big cells. |
| **Redirect** | 2 EP | Choose which board the next round is played in. It is marked NEXT. |
| **Claim** | 4 EP | Take a TIE board as your big cell. |

## Modes
- **vs CPU** with three levels: Easy, Normal and Hard. You play X.
- **2 Players** on the same device. Both players get buffs.

## Run it
Open `index.html` in a browser. There is no build step and no dependencies.
The page loads one web font (Press Start 2P) from Google Fonts and falls back to a monospace font if it is blocked.

## Host it
Any static host works, for example GitHub Pages, itch.io, Netlify or Cloudflare Pages. Upload `index.html` as it is.
