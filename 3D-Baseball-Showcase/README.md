# **Premium Baseball Showcase**

An ultra‑premium, interactive 3D landing page and design studio crafted to showcase limited‑edition collector’s baseballs. 

---

## **🌟 Key Features**

### **Interactive 3D WebGL Canvas**
A highly optimized, procedurally textured 3D baseball rendered using **Three.js**.  
Users can hover, grab, and drag to rotate and examine the ball from any angle.

### **Four Curated Collector‑Grade Styles**
- **The Classic 108** — Full‑grain off‑white leather with crimson double‑needle stitching.  
- **The Vintage Heirloom** — Distressed beeswax chestnut leather bound with rustic hemp cords.  
- **The Aurum Premier** — 24K gold electroplated shell with hand‑carved obsidian seam structures.  
- **The Lumina Night‑Ball** — Cybernetic polymer with neon UV‑reactive channels.

### **GSAP & ScrollTrigger Animations**
Smooth scroll‑bound transitions that:
- Morph materials  
- Rotate the ball to highlight specific facets  
- Adjust lighting profiles  
- Reflow typography layouts  

### **Web Audio API Sound Synthesizer**
Zero‑dependency, procedurally generated sound effects:
- **Bat Crack** — Fast pitch‑decayed sine oscillator blended with high‑pass noise.  
- **Seam Whoosh** — White noise shaped through a sweeping bandpass filter.

### **Bespoke Design Studio**
A slide‑out customization drawer enabling real‑time adjustments to:
- Leather coatings  
- Hex color palettes  
- Stitch materials  
- Roughness & metalness  
- Glow and luminescence  

---

## **📐 Mathematical Formulation of the Seam**

To ensure perfect visual fidelity without external texture maps, the baseball’s stitches are mathematically mapped onto a 3D sphere.

The seam follows a modified parametric infinity curve (similar to a spherical clelie curve) with scale factor \( a = 0.58 \) and radius \( R \), for \( t \in [0, 2\pi] \):

\[
x = R \cos(t) \sqrt{1 - a^2 \cos^2(2t)}
\]

\[
y = R \sin(t) \sqrt{1 - a^2 \cos^2(2t)}
\]

\[
z = R a \cos(2t)
\]

Stitch blocks are instanced along this curve using `THREE.InstancedMesh`, with tangent and normal vectors computed dynamically to orient each stitch in a traditional alternating V‑pattern.

---

## **🔊 Synthetic Audio Architecture**

A native synthesizer built on the **Web Audio API** replaces heavy audio assets.

### **Whoosh Effect**
- White noise buffer  
- Exponential bandpass sweep from **100 Hz → 1400 Hz**  
- Simulates aerodynamic compression around spinning seams  

### **Crack Effect**
- Pitch‑decayed sine oscillator (**900 Hz → 120 Hz**)  
- High‑pass filtered noise burst  
- Mimics the resonant impact of an ash‑wood bat  

---

## **🛠️ Technology Stack**

- **Render Pipeline:** Three.js (r128)  
- **Motion & Scroll Engine:** GSAP 3 + ScrollTrigger  
- **Styling & Layout:** Tailwind CSS  
- **Audio Synthesis:** Web Audio API  
- **Typography:** Google Fonts (Cinzel & Montserrat)  
- **Iconography:** FontAwesome 6  

---

## **🚀 Quick Start**

This project is a fully self‑contained **Single Page Application (SPA)** with no build step required.

1. Clone or download the project files.  
2. Ensure `index.html` is in the root directory.  
3. Open `index.html` in any modern browser (Chrome, Safari, Edge, Firefox).  
4. For best WebGL and audio performance, run via a lightweight local server:

   ```bash
   python -m http.server
   ```

---

## **📂 Project Structure**

```
├── index.html       # Unified SPA (HTML, CSS, JS)
└── README.md        # Documentation and design brief
```
---

## **🏃 Getting Started**

### **1. Download or Clone**

```bash
git clone https://github.com/JavascriptDon/Gemini-AI-Projects.git
cd Gemini-AI-Projects
```

### **2. Run Locally**

You can open `index.html` directly in any modern browser.

Or run a lightweight static server:

```bash
python3 -m http.server 8000
```

Then visit:

```
http://localhost:8000
```

---

## **🤝 Contributing**

Contributions are welcome.  
Please open an issue or submit a pull request with clear descriptions of changes.

---

## **📜 License**

This project is under the MIT License (MIT). See the LICENSE for more information.
