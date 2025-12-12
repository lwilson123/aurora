🌌 Aurora Arcade

A clean, Aurora-themed unblocked games hub powered by static HTML + a simple games.json file.

✨ Features

🎮 Games Library – Searchable grid of game cards with thumbnails

⭐ Favorites – Star games, saved in the browser

📂 JSON-Driven – Add/remove games just by editing games.json

🧩 Embedded Viewer – Games open inside load.html with fullscreen

🌑 Aurora Dark Theme – Unified UI across all pages

⚡ Lightweight – Perfect for school Chromebooks

🚀 Deploy Anywhere – GitHub Pages, Replit, etc.

🗺️ Project Structure
aurora/
├── index.html          # Landing page
├── load.html           # Game viewer
├── games/
│   ├── index.html      # Games library page
│   ├── games.json      # Game definitions
│   └── assets/         # Game folders + images
│       └── <game-name>/
│            ├── index.html
│            └── ...game files
└── README.md

🎮 How Aurora Arcade Works
1. Games Page (/games/)

Loads all games from games.json

Renders each card with:

Thumbnail

Title

Favorite star

Clicking a card loads:

/load.html?game=assets/<folder>/index.html&name=Your+Game

2. Game Player (load.html)

Displays game inside an iframe

Includes:

Fullscreen

Reload

Path display

Navbar that marks “Games” as active

🕹️ Adding a New Game

Create a folder inside:

/games/assets/<mygame>/


Put the game files inside (must include an index.html)

Add an entry to games/games.json:

{
  "name": "My Cool Game",
  "image": "assets/mygame/icon.png",
  "html": "assets/mygame/index.html"
}


✔ Paths are relative to /games/
✔ Make sure your image exists

🚀 Deploy on Replit

Click the button:

Steps

Replit imports your repo

If needed, create a basic static web server

Click Run

Open the generated web preview

🌐 Deploy on GitHub Pages

Go to Settings → Pages

Set:

Source: Deploy from branch

Branch: main

Folder: / (root)

Save

Your site will appear at:

https://<username>.github.io/<repo>/


For you:

https://lwilson123.github.io/aurora/

🧪 Local Testing (optional)

Run a local web server—this avoids iframe restrictions:

python -m http.server 8000


Then open:

http://localhost:8000

⭐ Favorites Storage

Stored using localStorage

Key: aaFavs

Clearing browser data resets favorites

🧱 Tech Stack

HTML

CSS

JavaScript

Zero backend

Fully static + portable

🔮 Future Ideas

Genre filtering

Recently played list

Themes selector

Custom game banners

Save states / notes per game

🎨 Credits

Made for fun — fast, clean, and optimized for students who love browser games.
Enjoy Aurora Arcade! 🌌🎮

If you want, I can also make:

✅ A Shields.io badge set
✅ A banner image for the top of your README
✅ A centered layout version
✅ A "Powered by Aurora Engine" footer

Just tell me!
