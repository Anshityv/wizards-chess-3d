# ♟️ 3D Wizard's Chess (Minimalist Gothic M3)

A fully playable, interactive **3D Wizard’s Chess** web application built entirely from scratch with zero external 3D model dependencies. Rendered via **Three.js** inside a procedural minimalist Gothic cathedral, complete with custom procedural piece animations, physics-driven shatter captures, and a single-level **Material Design 3 (M3)** HUD.

![Wizard's Chess Preview](https://images.unsplash.com/photo-1529699211952-734e80c4d42b?auto=format&fit=crop&w=1200&q=80) <!-- Optional atmospheric banner -->

---

## ✨ Key Features

- **Procedural Gothic Environment:** Soaring pointed arches, ribbed vaults, slate stone flooring, and volumetric lancet god-rays (`THREE.FogExp2`).
- **PBR Materials:** 
  - *White Side:* Polished Carrera marble (`MeshPhysicalMaterial` with subsurface scatter, clearcoat `0.8`).
  - *Black Side:* Volcanic obsidian (`MeshPhysicalMaterial` with high specular reflectivity and purple/blue tints).
- **4-State Piece Animation Machine:**
  - *Idle:* Asynchronous floating/breathing motions and royal aura sways.
  - *Move:* Parabolic gliding trajectories across the 64-square grid.
  - *Attack:* Dramatic wind-up strikes prior to capture.
  - *Shatter:* Physics-driven Voronoi shard explosions (20+ pieces bouncing with gravity and angular momentum on impact).
- **Complete Game Engine:** Powered by `chess.js` for full legal move validation, check/checkmate detection, and an intelligent heuristic AI opponent.
- **Single-Level M3 HUD:** Glassmorphic control bar (`backdrop-filter: blur(20px)`) housing live turn indicators, camera preset chips (Marble POV, Obsidian POV, Top-Down, Cinematic Orbit), mode toggles, and captured piece counters.

---

## 🚀 How to Run Locally

Because this project is packaged as a **single self-contained HTML file**, running it takes less than 30 seconds with zero build steps or package installations required!

1. **Copy the Code:** Copy the complete HTML source code provided in the project.
2. **Create the File:** Create a new file on your computer named `index.html` and paste the code inside.
3. **Open in Browser:** Double-click `index.html` to open it directly in any modern browser (Chrome, Safari, Firefox, Edge). 

*(Note: An active internet connection is required on first load as it pulls Three.js, OrbitControls, and Chess.js directly via CDN).*

---

## 🛠️ Built With

- **Three.js (r128)** — 3D WebGL rendering, lighting, and materials.
- **OrbitControls** — Smooth camera navigation and preset transitions.
- **Chess.js** — Game logic, move generation, and state validation.
- **Google Fonts & Material Symbols** — Material Design 3 typography and iconography.

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).
