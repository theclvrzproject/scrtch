# **scrtch**
A simple, fast, and open archive for **Scratch games**, preserved and delivered as **TurboWarp-compiled HTML projects**.

Inspired by the idea behind the open-source project archive *gfiles*, **scrtch** aims to provide a centralized, self-hostable place where Scratch creations can live forever—easy to browse, easy to play, and easy to add more.

---

## 🚀 **About**
**scrtch** is a lightweight web-based collection of Scratch projects that have been exported or compiled through **TurboWarp Packager** into standalone HTML files.

This project exists to:
- Preserve Scratch games in a playable format  
- Remove loading delays and dependencies from scratch.mit.edu  
- Offer an offline-friendly and embeddable alternative  
- Provide a simple structure for contributors to add more games over time  

It is **not** affiliated with Scratch, the Scratch Team, or MIT.

---

## 📦 **Adding a Game**
1. Export your Scratch project using **TurboWarp Packager**  
   - https://packager.turbowarp.org  
   - Recommended settings:  
     - FPS: 60  
     - “Remove Project ID” enabled  
     - “Zip project” to download a folder-compatible version  

2. Create a new folder inside `/games/` with a clear name:  
   ```
   games/project-name/
   ```

3. Place the exported **HTML** and asset files inside that folder.

4. Add an entry to `data/games.json`:
   ```json
   {
     "id": "project-name",
     "title": "Project Title",
     "author": "Creator Name",
     "thumbnail": "assets/project-name.png",
     "description": "Short description of the project."
   }
   ```

5. (Optional) Add a thumbnail image under `/assets/`.

6. Open `index.html` or `[gamename].html` to verify the game appears properly.

---

## 🎮 **Features**
- 🚄 **Fast loading** (TurboWarp optimized)
- 📂 **Self-hostable** — works on GitHub Pages, Cloudflare Pages, Netlify, or any static host
- 💾 **Offline-friendly** — all HTML games are stored locally
- 🔍 **Searchable & browsable** list of games
- 💬 Optional metadata files for better indexing

---

## 🔧 **Requirements**
No build system required.  
Just a static web host or local filesystem.

---

## 🤝 **Contributing**
Contributions are welcome!  
You can help by:
- Adding more Scratch games  
- Improving UI/UX  
- Enhancing the search system  
- Fixing performance or compatibility issues  

Open a pull request and follow the structure outlined above.

---

## 📜 **License**
MIT License (or whichever you choose).  
Scratch projects remain property of their respective creators.  
TurboWarp is licensed separately—see its project page for details.
