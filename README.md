# Mr. Do!

A faithful browser-based recreation of the classic 1982 arcade game. Dig through dirt, collect cherries, crush enemies with apples, and throw your bouncing ball to clear each level.

## How to Play

Open `index.html` in any modern web browser. No installation, server, or dependencies required — everything runs in a single self-contained HTML file.

## Controls

### Keyboard

| Key | Action |
|-----|--------|
| **Arrow Keys** or **WASD** | Move / dig through dirt |
| **Space** or **Z** | Throw ball |
| **Enter** | Confirm (high score entry) |

### Touch (Mobile)

- **D-pad** (bottom-left): Movement
- **Fire button** (bottom-right): Throw ball

## Objectives

Each level can be completed in three ways — you only need to achieve one:

1. **Collect all cherries** — gather every cherry on the field
2. **Kill all enemies** — eliminate every enemy using your ball or apples
3. **Spell EXTRA** — collect all five letters from alpha monsters to earn an extra life and clear the level

## Game Elements

### Your Ball

Your primary weapon. Press Space/Z to throw it in the direction you're facing.

- Bounces off walls and dirt (up to 14 bounces)
- Kills any enemy it touches
- Returns to you after hitting an enemy or running out of bounces
- **Regeneration delay increases** with each throw — use it wisely

### Cherries

Pink collectibles found in groups of 8 scattered around each level.

| Action | Points |
|--------|--------|
| Collect one cherry | 50 |
| Collect a full group of 8 | 500 bonus |

### Apples

Green hazards that can be used as weapons.

- Sit on top of dirt — if you dig the dirt beneath them, they wobble and fall
- Crush enemies underneath for big points
- **Be careful** — falling apples kill you too

| Enemies Crushed | Points |
|-----------------|--------|
| 1 | 1,000 |
| 2 | 2,000 |
| 3 | 4,000 |
| 4 | 6,000 |
| 5+ | 8,000 |

### Enemies

Enemies spawn from the generator in the centre of the field.

- **Standard enemies** — chase you through tunnels using pathfinding
- **Diggers** — standard enemies transform into diggers after ~18 seconds; these can carve through dirt to reach you
- **Alpha monsters** — yellow enemies that appear at every 5,000 points, carrying one letter of EXTRA. Kill them with your ball to collect the letter. Worth 1,000 points.

Enemy count increases with each level (minimum 4, up to 18 at higher levels).

### EXTRA Letters

A rotating letter display at the top of the screen cycles through E-X-T-R-A. Collect all five letters from alpha monsters to earn an extra life.

## Lives

- You start with **3 lives**
- Lose a life when hit by an enemy or a falling apple
- Gain a life by spelling EXTRA
- After dying, you respawn with brief invincibility (flashing)

## Levels

The game has 8 unique level layouts that cycle, each with a different dirt colour theme (green, brown, blue, purple, gold, crimson, teal, olive). Difficulty increases with each level — enemies get faster and more numerous.

## High Scores

- Top 10 scores are saved in your browser's local storage
- If you qualify, you'll be prompted to enter 3-letter initials
- Use **Up/Down** to change letters, **Left/Right** to move between positions, **Enter** to confirm
- You can also type letters directly

## Sound

All sound effects and music are synthesised in real-time using the Web Audio API — no audio files are loaded. The soundtrack is a chiptune rendition of Offenbach's Can-Can.

## Browser Requirements

Any modern browser with HTML5 Canvas and Web Audio API support (Chrome, Firefox, Safari, Edge). Works on desktop and mobile.

---

Mr. Do! is provided by [Jorvik Software](https://jorviksoftware.cc/). If you find it useful, consider [buying me a coffee](https://jorviksoftware.cc/donate).
