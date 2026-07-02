# Backrooms Labirynth

Co-op (1–4 players) escape-room horror set in the Backrooms, rendered like a lost PS1 game. One HTML file, no build step.

**PLAY: https://jerzysukiennik.github.io/backrooms-labirynth/**

## What it is

You wake up in Level 0. Between you and the exit gate stand up to 15 rooms, each locked behind a colored door and each hiding its key behind a different physics puzzle — topple a tower, assemble a rocket, dig in the grass, drive cars into color-matched garages, count the legs of wandering animals in a pastel Level 94 town, read a code through a real mirror, weigh scrap on a scale, flip breakers in the order the lamps blink, dive into a ball pit, or crawl through a room where someone stole the light. Seat every key by the gate and step into the machine world on the other side.

- **Multiplayer:** host-authoritative WebRTC P2P (Firebase RTDB is used only for signaling), room codes, per-player wallets, unique avatar colors, mid-run rejoin.
- **Physics:** Rapier 3D — every piece of furniture, key, coin, ball and car is a real rigid body. Human-Fall-Flat-style grab and throw, one free hand.
- **PSX pipeline:** low-res render target, vertex snapping, affine texture warp, Gouraud vertex lighting, dither and grain.
- **No monsters.** The horror is the presence: light dips, whispers, knocks, silhouettes, haunted counters.
- Solo checkpoint saves, quality/volume settings, photo mode `[P]`, PL/EN.

## Controls

| | |
|---|---|
| WASD / Space / Ctrl / Shift | move · jump · crouch · sprint |
| Hold LMB | grab (one hand) |
| F | throw |
| E | use · sit · get in a car |
| T / H | toggle held light / headlamp |
| RMB | ping marker |
| P | photo mode |
| ESC | pause, settings and a hint if you are stuck |

## Repository layout

Each `vX.Y/` folder is a frozen milestone build — the full history of the project, newest last. The root `index.html` redirects to the current release.

Run locally: serve any version folder over HTTP (e.g. `python3 -m http.server`) and open it — WebRTC and audio need a real origin, not `file://`.

Made by **Jurek** (GSP) with Claude.
