# SolidWorks 3D Anti-Gravity Room Visualizer

An interactive 3D web visualizer built with **Three.js** that renders your room with exact measurements (**2.77m Width × 5.13m Length × 2.70m Height**) and simulates real **anti-gravity / zero-gravity physics** for your SolidWorks CAD designs.

## Features
- **Accurate Room Architecture:** Exact dimensions from your room sketch ($277\text{ cm} \times 513\text{ cm}$), complete with the window venetian blinds, left-wall office table, drawers, tall filing cabinet, and sink fixtures matching your room photos.
- **SolidWorks Import Pipeline:** Drag and drop or upload `.STL` or `.GLB` files directly into the web app.
- **Physical Collision Bounds:** CAD parts bounce naturally off the cream drywall, vinyl floor, drop-ceiling, and the office table.
- **Anti-Gravity Physics Engine:** Adjust effective gravity from $-9.8\text{ m/s}^2$ (floating up to ceiling) to $0.0\text{ m/s}^2$ (pure weightless zero-g) and $+9.8\text{ m/s}^2$ (standard gravity). Includes microgravity turbulent drift, rotational momentum, and drag damping.
- **Click & Fling:** Grab any CAD part in mid-air with your mouse or touch screen and toss it across your room.

---

## Deploying to Vercel (Free & Instant)

### Option 1: Via Vercel CLI (Fastest)
1. Unzip this package.
2. In your terminal, navigate inside the unzipped folder:
   ```bash
   cd cad-room-antigravity
   ```
3. Deploy directly using the Vercel CLI:
   ```bash
   npx vercel
   ```
4. For instant production deployment:
   ```bash
   npx vercel --prod
   ```

### Option 2: Via GitHub + Vercel Web Dashboard
1. Create a new repository on GitHub (e.g., `cad-room-antigravity`).
2. Push this folder to GitHub:
   ```bash
   git init
   git add .
   git commit -m "SolidWorks Room Anti-Gravity Visualizer"
   git branch -M main
   git remote add origin https://github.com/<your-username>/cad-room-antigravity.git
   git push -u origin main
   ```
3. Open [vercel.com](https://vercel.com) and click **"Add New Project"**.
4. Import your GitHub repository and hit **Deploy**.

---

## How to Export from SolidWorks
1. **Direct STL Export:**
   - In SolidWorks: `File` → `Save As...` → choose `STL (*.stl)`.
   - Click `Options...`: set output to **Binary** and deviation/tolerance to **Fine**.
   - Upload the `.stl` file directly into the visualizer using the panel button.
2. **GLB with Colors / Materials:**
   - Save your assembly in SolidWorks as `STEP AP214 (*.step)`.
   - Import the `.step` into Blender or use an online CAD converter to export as `.glb`.
   - Drop the `.glb` into the visualizer.
