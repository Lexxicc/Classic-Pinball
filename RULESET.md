# Classic Pinball — Ruleset

> Keep this file in sync with the How to Play page in `Classic Pinball.html` whenever rules or mechanics change.

---

## Goal

Keep the ball alive and rack up the highest score before losing all **5 balls**. Every hit is multiplied by a rally bonus that builds the longer your ball survives.

---

## Controls

| Input | Action |
|---|---|
| Tap left half of screen / ← / Z | Left flipper |
| Tap right half of screen / → / / | Right flipper |
| Either paddle (ball inactive) | Launch ball |

**Launch direction:**
- Left paddle → ball fires up-right (45°)
- Right paddle → ball fires up-left (315°)

---

## Bumpers

10 bumpers drift slowly around the board, bouncing off walls.

| Hit | Points |
|---|---|
| First hit on a bumper | 100 pts |
| Repeat hits on same bumper | +50 pts each |
| Hit all 10 bumpers in one ball | +1,000 bonus (all-clear) |
| Top lane (ball reaches top with upward velocity) | +750 pts (once per ball) |

All points are multiplied by your current **rally multiplier**.

---

## Rally Multiplier

- Starts at **×1.0** when a new ball is launched
- Increases **+0.25×** every ~10 seconds
- Maximum: **×3.0**
- Resets to **×1.0** when the ball is lost

---

## Ball Physics

- **5 balls** per game
- Gravity pulls the ball downward continuously
- Slight air drag applied each frame
- Speed capped at 17 px/s to prevent tunnelling
- Hitting an active (pressed) flipper boosts ball speed ×1.4

---

## Game Over

When all 5 balls are lost, the game ends. Score is saved to the leaderboard.

Tap either side of the screen to restart.

---

## Scoring Summary

All base point values (100, 50, 750, 1000) are multiplied by the current rally multiplier before being added to your score.

---

Last updated: 2026-05-02 — v0.0.3
