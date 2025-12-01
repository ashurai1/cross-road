# Road Cross

Simple 3D arcade game built with `three` and vanilla JS. Guide the player across an endless road, avoid cars and trucks, and rack up your score one row at a time.

## Features
- Orthographic camera with dynamic viewport
- Procedural rows (grass, roads, trees, vehicles)
- Smooth player movement and rotation animations
- Collision detection with vehicles and game-over UI
- Keyboard and on-screen controls

## Tech Stack
- `three` loaded via ESM CDN (`https://esm.sh/three`)
- Vanilla JavaScript, HTML, and CSS

## Project Structure
- `dist/` — runnable build for the browser (`index.html`, `script.js`, `style.css`)
- `src/` — source files for development

## Run Locally
You can open the game directly or serve it via a static server.

Option 1: open file directly
- Open `dist/index.html` in your browser

Option 2: run a simple static server (recommended)
- `cd dist`
- `python3 -m http.server 8000`
- Open `http://localhost:8000/` in your browser

## Controls
- Keyboard: Arrow keys (`↑`, `↓`, `←`, `→`)
- UI Buttons: Click the on-screen arrows

## Gameplay
- Move forward to increase your score
- Avoid cars and trucks; collisions show the Game Over dialog with your final score
- Click `Retry` to restart

## Implementation Notes
- Keyboard and button controls are wired in `src/script.js:683-713`
- Collision detection runs each frame in `src/script.js:715-736`
- Vehicle animation and recycling are handled in `src/script.js:652-681`

## Deploy to GitHub Pages
If your repo is on GitHub, you can deploy the `dist/` directory:
- Push your repository to GitHub
- Go to `Settings` → `Pages`
- Set `Source` to `Deploy from a branch`
- Choose your default branch (e.g., `main`) and folder `/dist`
- Save; wait for the site to build and publish



## Copyright
Copyright (c) 2025 Ashwani Rai. All rights reserved.
