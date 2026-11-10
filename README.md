# My own IGI browser build

My own hosted copy of the **OpenIGI web build v0.6.7** — Project I.G.I. in the
browser, on my own GitHub Pages site. Not openigi.com, not playigi.com.

Live site: **https://authorityspoke.github.io/igi-browser/**

## Code only — no game assets

This repo contains **code only**. It includes no game files from Project I.G.I.:

- No `IGI.exe`
- No `.res`, `.qvm`, `.iff`, `.tex`, `.dat`, `.mtp` or `.mef` game files
- No levels, missions, textures, models or sounds from the game
- No files from any installed IGI folder

The only assets shipped are OpenIGI's own web-build assets (its fonts,
colour LUTs, rain-loop sound and UI files) that come with the upstream
OpenIGI v0.6.7 release.

## How to play

1. Open https://authorityspoke.github.io/igi-browser/ in a current
   Chrome, Edge or Safari browser. **WebGPU is required.**
2. When the game asks, pick your own installed Project I.G.I. folder —
   the folder with `IGI.exe` in it (usually the `PC` folder). The files
   are read locally in your browser and are never uploaded.
3. Pick a mission. The browser build covers the **first 6 missions**,
   with the original (vanilla) graphics. No multiplayer in the browser
   build.

## Source

- Engine: OpenIGI (https://github.com/OpenIGI/OpenIGI), clean-room
  reimplementation of Project I.G.I. (2000), **GPL-3.0**
- Web build: OpenIGI v0.6.7, prebuilt release, hash-verified against the
  release `SHA256SUMS` before publishing here
- Game data: supplied by each player from their own copy of the game,
  at runtime, in their own browser. Nothing is bundled here.

Project I.G.I. is © Innerloop Studios / Eidos Interactive (2000).
This is a fan-hosted build of the open-source OpenIGI engine, not
affiliated with or endorsed by them.
