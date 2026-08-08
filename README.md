# Echo

**A sonar puzzle-platformer told entirely in the dark.**

Built for the LevelUp Game Hackathon 2026 (Gamnexis) by **Team LevelUp Raiders**.

---

## Team

| Name | Role |
|---|---|
| Harish Reddy Devapatla | Team Lead — mechanics & architecture |
| Uday Kiran Akkannagari | Level design & art |
| Asif PMd | Audio, QA & submission assets |

---

## About the Game

You navigate total darkness using only brief pulses of light. Press **Space** to emit a pulse — it briefly reveals nearby platforms, hazards, and enemies before fading back to black. You have to memorize what you saw and move on trust.

Across 3 levels, the challenge escalates:

1. **Level 1 — First Light**: pure navigation, no threats. Learn the mechanic.
2. **Level 2 — Something Listens**: enemies react to your pulses and give chase if alerted.
3. **Level 3 — The Last Charge**: a limited pulse-energy meter forces you to ration every reveal.

## Controls

| Key | Action |
|---|---|
| `Arrow Keys` / `WASD` | Move |
| `Up` / `W` | Jump |
| `Space` | Emit pulse |
| `R` (on win screen) | Play again |

## Features

- Real-time lighting via Phaser 3's Lights2D pipeline — the reveal effect is a genuine dynamic light, not a static overlay trick
- Hand-tuned gradient art (player, platforms, enemies, hazards, goal beacon) rendered via canvas gradients — no flat placeholder shapes
- Animated title screen with expanding pulse rings and a glowing logo
- Ambient dust particles and a soft vignette for atmosphere
- Particle burst + camera shake on every pulse for feedback
- Sound-reactive enemy AI that shifts from idle patrol to active chase when alerted
- A pulse-energy resource system that turns every reveal into a risk/reward decision
- Styled HUD with a level-progress indicator
- Instant browser play — no install, no build step

## Tech Stack

- **Engine/Framework:** Phaser 3 (v3.70.0)
- **Language:** JavaScript (ES6+)
- **Rendering:** HTML5 Canvas via Phaser's WebGL/Canvas renderer + Lights2D pipeline
- **Hosting:** GitHub Pages
- All art (platforms, player, enemies, hazards) is generated procedurally in code — no external image assets required

## Run It Locally

No build step needed. Either:

- Open `index.html` directly in a modern browser (Chrome/Firefox/Edge), **or**
- Serve the folder locally for best results:
  ```bash
  npx serve .
  # then visit the printed localhost URL
  ```

## Play It Online

▶ **[Play Echo in your browser](#)** *(replace with your deployed GitHub Pages / Netlify link before submitting)*

## Project Structure

```
echo/
├── index.html      # entire game — Phaser scenes, level data, and game logic
└── README.md        # this file
```

## AI Usage Declaration

AI tools (Claude, Anthropic) were used to help structure the project proposal, brainstorm the core concept, and assist with drafting/debugging the Phaser 3 implementation. All final game design decisions, level design, and tuning were made and verified by the team, who can explain and defend every part of the implementation.

## License / Submission Note

This project was built primarily during the LevelUp Game Hackathon 2026 for submission to Gamnexis. All assets are original or procedurally generated.
