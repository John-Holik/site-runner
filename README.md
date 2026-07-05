# Site Runner

Chrome-dino-style endless runner with a construction-safety learning layer. Drive a construction vehicle across a night-shift job site, **jump** ground hazards (cones, trenches, pallets) and **duck** low clearances (scaffold bars, duct runs). Checkpoint questions are the coin economy: correct answers pay an escalating streak and restore a hard hat; collisions are HR-friendly near-misses, never deaths.

Single self-contained HTML file (Phaser 3 via CDN, all textures generated at runtime). No build step, no assets.

## Play

Open `site-runner.html` in a browser.

- SPACE / ↑ / tap right = jump · ↓ hold / hold left = duck · P/ESC = pause
- **Garage** — 7 unlockable vehicle skins
- **Training Yard** — Duck Life-style persistent stats: ENGINE (top speed), THROTTLE (ramp-up), PLATING (extra hard hats)
- Difficulty modes (Rookie / Crew / Veteran), day/night themes, XP/rank profile with question mastery and per-category accuracy

## Custom questions

Questions are **uploaded, not coded**: CSV or JSON from the menu (persisted to `localStorage`). A 51-question sample bank (OSHA Focus Four + electrical/fire/PPE/general) is bundled; starter files in `templates/`.

`instructor.html` is a companion authoring tool: create/edit/import/export questions with validation and in-game-style preview, then install the bank directly into the game. It also carries the self-test harnesses (`?selftest=1`, `?domtest=1`).
