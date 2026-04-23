# Chaos Connect 4 — Human vs AI

A single-file web game built for **Innovation Friday: Human vs AI**.

Standard Connect 4 rules (7×6, four-in-a-row wins) — but every ~3 turns, **CHAOS** strikes and the rules change on you.

## Chaos Events

- **Gravity Flip** — next drop falls upward
- **Column Shuffle** — all 7 columns are randomly reordered (stacks preserved)
- **Blind Move** — board is blurred for 2 seconds before your move
- **Double Drop** — current player drops twice this turn
- **Row Clear** — the bottom row is wiped and everything settles

## Features

- Heuristic AI (win → block → center/threat scoring), responds < 500ms
- Animated piece drops, dark + neon-green theme
- AI trash talk reacts to win/loss state
- Chaos log, persistent win/loss score, sound toggle (WebAudio)
- Start screen → game → restart loop

## Run

Just open `index.html` in any modern browser. No dependencies, no build.

```bash
xdg-open index.html
# or
python3 -m http.server 8000
```

## Controls

- **Hover** a column to highlight, **click** to drop.
- Top-right `🔊 SOUND` toggles audio.
- `reset` next to the score clears the scoreboard.
- `◀ MENU` returns to the start screen.
