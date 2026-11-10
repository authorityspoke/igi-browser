# My own IGI browser build

My own hosted copy of the **OpenIGI web build, built from source** — Project
I.G.I. in the browser, on my own GitHub Pages site. Not openigi.com, not
playigi.com.

Live site: **https://authorityspoke.github.io/igi-browser/**

## Code only — no game assets

This repo contains **code only**. It includes no game files from Project I.G.I.:

- No `IGI.exe`
- No `.res`, `.qvm`, `.iff`, `.tex`, `.dat`, `.mtp` or `.mef` game files
- No levels, missions, textures, models or sounds from the game
- No files from any installed IGI folder

The only assets shipped are OpenIGI's own web-build assets (its fonts,
colour LUTs, rain-loop sound and UI files) that come with the upstream
OpenIGI source.

## How to play

1. Open https://authorityspoke.github.io/igi-browser/ in a current
   Chrome, Edge or Safari browser. **WebGPU is required.**
2. When the game asks, pick your own installed Project I.G.I. folder —
   the folder with `IGI.exe` in it (usually the `PC` folder). The files
   are read locally in your browser and are never uploaded.
3. Pick a mission. The browser build covers the **first 6 missions**.
   No multiplayer in the browser build.

## Graphics — changeable later

The build starts on the **vanilla** preset (the original's look, and the
lightest — the phone default; touch devices also render at 0.75 scale).
To raise the graphics later, add one of these to the address — no
rebuild needed:

- `?preset=enhanced`, `?preset=high` or `?preset=ultra`
- `?scale=0.8` renders below the screen for speed (0.25–1)

Example: `https://authorityspoke.github.io/igi-browser/?preset=high`

## Source

- Engine: OpenIGI (https://github.com/OpenIGI/OpenIGI), clean-room
  reimplementation of Project I.G.I. (2000), **GPL-3.0**
- Web build: built from the OpenIGI source at commit `e3af23c` with the
  .NET 10 SDK (10.0.301) + `wasm-tools` workload. The only changes from
  upstream are the graphics options above (`?preset=` / `?scale=`,
  phone default), in `apps/OpenIGI.Web` (`Program.cs`, `wwwroot/main.js`,
  `wwwroot/index.html`).
- Game data: supplied by each player from their own copy of the game,
  at runtime, in their own browser. Nothing is bundled here.

Project I.G.I. is © Innerloop Studios / Eidos Interactive (2000).
This is a fan-hosted build of the open-source OpenIGI engine, not
affiliated with or endorsed by them.
