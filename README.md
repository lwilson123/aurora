# 🌌 Aurora Arcade

> A clean, Aurora–themed unblocked games hub powered by static HTML + a simple `games.json` file.

[![Run on Replit](https://replit.com/badge/github/lwilson123/aurora)](https://replit.com/new/github/lwilson123/aurora)

---

## ✨ Features

- 🎮 **Games Library** – Searchable grid of game cards with thumbnails  
- ⭐ **Favorites** – Star games, saved locally in your browser  
- 📂 **JSON‑Driven** – Add/remove games just by editing `games.json`  
- 🧩 **Embedded Player** – Games open inside a stylish iframe on `load.html`  
- 🌓 **Aurora Dark Theme** – Matching landing page + games page UI  
- 🏫 **Static & Lightweight** – Ideal for Chromebooks + school networks  

---

## 🗺️ Project Structure

```text
.
├── index.html          # Landing / home page
├── load.html           # Game player (iframe loader)
├── games/
│   ├── index.html      # Games library page
│   ├── games.json      # Game definitions (name, image, html)
│   └── assets/         # Game folders live here
│       ├── mygame1/
│       │   ├── index.html
│       │   └── ...game files...
│       └── mygame2/
│           ├── index.html
│           └── ...
└── README.md
🎯 How It Works
1. Games Library (/games/index.html)
Reads games/games.json
Renders cards with:
cover image (icon)
title
favorite button (★)
Clicking a card sends you to load.html with the game info in the URL.
text
Copy code
/load.html?game=assets/mygame1/index.html&name=My+Game+1
2. Game Player (/load.html)
Reads game + name from the query string
Loads /games/<game> into an iframe
Has:
Reload button
Fullscreen button
Top nav with “Games” active
🕹️ Adding Games
All games are defined in games/games.json.
Example games.json
json
Copy code
{
  "games": [
    {
      "name": "Drive Mad",
      "image": "assets/drivemad/icon.png",
      "html": "assets/drivemad/index.html"
    },
    {
      "name": "1v1.lol",
      "image": "assets/1v1/icon.png",
      "html": "assets/1v1/index.html"
    }
  ]
}
Rules
image and html paths are relative to /games/
If your game lives at:
/games/assets/drivemad/index.html
then your JSON should use:
json
Copy code
"html": "assets/drivemad/index.html"
Place all game folders inside games/assets/.
🚀 Deploy to Replit
Click this button to clone and run Aurora Arcade on Replit: 
On Replit
Click the badge above.
Wait for Replit to import the repo.
If it doesn’t auto-detect, create a simple index.html run configuration:
Make sure the “Run” command starts a static web server or uses Replit’s built-in web view.
Press Run – your site should open in the right-hand preview / web tab.
🌐 Deploy to GitHub Pages
Push this repo to GitHub (you already did: lwilson123/aurora).
In the repo settings:
Go to Pages
Set:
Source: Deploy from a branch
Branch: main → / (root)
Your site will be available at:
text
Copy code
https://lwilson123.github.io/aurora
index.html → landing page
/games/ → games library
/load.html → game player
🧪 Local Testing (optional)
If you want to run it locally with a simple static server:
bash
Copy code
# Python 3
python -m http.server 8000

# Then open:
# http://localhost:8000
# http://localhost:8000/games/
💾 Favorites Storage
Favorites are stored in the browser using localStorage.
Key name: auroraArcadeFavorites
Clearing site data / localStorage will reset favorites for that browser.
🧱 Tech Stack
HTML / CSS / JavaScript only
No frameworks
No build step required
Fully static, works on any static host (GitHub Pages, Replit, etc.)
✨ Ideas / To‑Do
⏱️ “Recently played” list
🏷️ Tags / genres & filters
🎨 Custom themes (Aurora color presets)
🧩 Per-game settings (volume, WASD arrows, etc.)
Made for fun as a clean, fast unblocked games launcher. 🎮🌌
makefile
Copy code
::contentReference[oaicite:0]{index=0}






