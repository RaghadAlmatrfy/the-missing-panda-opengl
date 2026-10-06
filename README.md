# 🐼 The Missing Panda — 2D OpenGL Animation

A short animated story built with **C++ and OpenGL (GLUT)**. A mother panda loses her baby near the lake and searches for him through the forest — through rain and wind — until they are finally reunited.

> *"Family is the most important thing."*

Computer Graphics (CS2206) course project — Umm Al-Qura University.

![Demo](demo.gif)

🎬 Full video: [demo.mp4](demo.mp4)

---

## 📖 Story & Scenes

| # | Scene | Preview |
|---|---|---|
| 1 | **Playtime** — the baby panda plays near the lake while ducks float on the water | ![Scene 1](scene1.png) |
| 2 | **The search begins** — the mother looks around with a worried face: *"Where is my baby?!"* | ![Scene 2](scene2.png) |
| 3 | **Asking for help** — she walks through the forest and asks a hopping rabbit: *"Have you seen my baby"* | ![Scene 3](scene3.png) |
| 4 | **The storm** — the weather changes: rain falls, trees sway in the wind, the background darkens | ![Scene 4](scene4.png) |
| 5 | **Reunion** — the mother finds her baby and hugs him as animated hearts appear | ![Scene 5](scene5.png) |

---

## ✨ Graphics Techniques Used

- **2D primitives** — all characters and objects (pandas, rabbits, ducks, trees, hearts) are built from circles, triangles and quads
- **Transformations** — translation (walking), rotation (head turning, swaying trees, spinning hearts) and scaling (lake, rabbit ears)
- **Hierarchical modeling** with `glPushMatrix` / `glPopMatrix`
- **Animation loop** using `glutTimerFunc` (~60 FPS) with `sin()`-based motion for floating ducks, hopping rabbit and pulsing hearts
- **Particle-style rain** using a vector of raindrops with random positions and speeds
- **Alpha blending** for fading hearts and transparent rain
- **Texture mapping** — BMP images loaded as background textures
- **Bitmap text** rendering for story dialogue
- **Keyboard interaction** to switch scenes

---

## ▶️ How to Run

**Requirements:** Visual Studio, FreeGLUT and GLEW.

1. Create a new C++ project in Visual Studio and add `main.cpp`.
2. Install/link **FreeGLUT** and **GLEW** (e.g. via NuGet: `nupengl.core`).
3. Place two 24-bit BMP background images next to the executable:
   - `background1.bmp` — sunny sky (720×510)
   - `background2.bmp` — rainy sky (1024×725)
4. Build and run.

### 🎮 Controls

| Key | Action |
|---|---|
| `1` – `5` | Switch between scenes |
| Close window | Exit |

---

## 📁 Files

| File | Description |
|---|---|
| `main.cpp` | Full source code |
| `demo.gif` / `demo.mp4` | Animation demo |
| `scene1.png` … `scene5.png` | Scene screenshots |
| `The_Missing_Panda_Report.docx` | Project report |
| `The_Missing_Panda_Presentation.pdf` | Presentation slides |
| `User_Manual.pdf` | User manual |

---

## 👥 Team

| Member | Contribution |
|---|---|
| Ethar Tamim | Panda models, environment (lake, trees, ducks), background texture — Scene 1 |
| Layan Alshreef | Scene 2 — mother searching (rotation, eyes, eyebrows, text) |
| Sama AlSilaimi | Scene 3 — panda walking, rabbit motion, duck wave animation, timed text |
| Munirah Ali Sulaiman | Scene 4 — weather change: rain, wind, rainy background |
| **Raghad Almatrfy** | Scene 5 — reunion, hug and animated hearts, final message |

Supervised by **Dr. Omniah H. Nagoor** — Umm Al-Qura University.
