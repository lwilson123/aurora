<div align="center">

# 🌌 **Aurora Arcade**
### The clean, modern unblocked game hub — powered by simple JSON and static HTML.

[![Run on Replit](https://replit.com/badge/github/lwilson123/aurora)](https://replit.com/new/github/lwilson123/aurora)

</div>

---

## ✨ Features

- 🎮 **Clean games library UI**
- ⭐ **Favorites system (saved locally)**
- ⚡ **Loads games inside an iframe viewer (load.html)**
- 📂 **Add games easily via games.json**
- 🎨 **Aurora dark theme**
- 🚀 **Fast + lightweight — works on school Chromebooks**

---

## 🗂️ Project Structure

aurora/
├── index.html
├── load.html
├── games/
│ ├── index.html
│ ├── games.json
│ └── assets/
│ └── <game-folder>/
│ ├── index.html
│ └── ...other files
└── README.md


---

## 🕹️ Adding a Game

1. Create your folder inside:

games/assets/<game-name>/

2. Make sure it contains `index.html`  
3. Add a JSON entry:

```json
{
  "name": "Cool Game",
  "image": "assets/coolgame/icon.png",
  "html": "assets/coolgame/index.html"
}
```
▶️ How Games Load


When you click a game card: load.html?game=assets/<folder>/index.html&name=Cool+Game
