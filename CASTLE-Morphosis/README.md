# **Castle Morphosis: Stylistic Progression Engine**

Castle Morphosis is an interactive single-page application (SPA) built with a custom-engineered HTML5 Canvas rendering pipeline. This application is built using Google Gemini from a single prompt, utilizing Tailwind CSS for its modern design, and contains zero external runtime script dependencies besides the styling framework.

## **🌐 Overview**

Castle Morphosis is a visual transformation engine that morphs uploaded images or predefined silhouettes through **four distinct artistic styles**, each implemented with custom procedural rendering techniques. The result is a fluid, tactile, and highly interactive visual experience that blends analog art with digital precision.


https://github.com/user-attachments/assets/11e739a4-9272-4ddf-b145-a4cb32a8b342


---

## **🚀 Features**

### **Interactive Tools**
- **Instant Image Upload**  
  Supports JPG, PNG, and WEBP. Automatically extracts grayscale shading, isolated colors, and Riso plates.

- **Split‑Screen Comparison**  
  Compare your current style with the next stage in real time.

- **High‑Resolution PNG Export**  
  Export your tuned render as a crisp, lossless PNG.

- **Live Parameter Controls**  
  Adjust wax density, line‑boiling rate, refraction index, Riso registration offset, and more.

- **Seamless Style Blending**  
  Dual offscreen buffers interpolate colors, alphas, and textures for smooth transitions.

---

## **🎨 Stylistic Stages**

### **1. Vibrant Crayon Aesthetic**
**Aesthetic Focus:** Playful, physical, organic warmth.

**Techniques**
- Waxy texture overlays  
- Stroke jitter for hand‑drawn irregularity  
- Granulated paper fiber noise  

---

### **2. Graphite Pencil Sketch**
**Aesthetic Focus:** Traditional fine‑art draftsmanship.

**Techniques**
- 12fps line‑boiling animation  
- Procedural cross‑hatching  
- Dynamic line‑weight variation  

---

### **3. 3D Translucent Glass Style**
**Aesthetic Focus:** Modern, hyper‑realistic minimalist rendering.

**Techniques**
- Refraction index pixel shifting  
- Volumetric shading gradients  
- Caustic lighting and soft glows  

---

### **4. Tactile Risograph Print**
**Aesthetic Focus:** Mid‑century mechanical printing.

**Techniques**
- 3‑color separation (Teal, Magenta, Yellow)  
- Registration misalignment simulation  
- Halftone dot matrix overlays  

---

## **🛠️ Technical Implementation**

- Built with **vanilla ES6+ JavaScript**  
- Uses `CanvasRenderingContext2D` for all rendering  
- **Fitted Image Math** ensures any aspect ratio fits a responsive **4:5 frame** without distortion  
- **Noise generation** uses safe integer bounds to avoid `IndexSizeError`  
- **Composite blending** uses native Canvas modes (`multiply`, `screen`, `source-atop`)  

---

## **📁 Project Structure**

```
/
├── index.html
└── README.md
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

## **🧭 Roadmap**

- [ ] Add mobile‑optimized parameter panel  
- [ ] Add preset gallery  
- [ ] Add animation export (GIF/WebM)  
- [ ] Add custom color palettes for Riso mode  
- [ ] Add WebGL acceleration for glass refraction  

---

## **🤝 Contributing**

Contributions are welcome.  
Please open an issue or submit a pull request with clear descriptions of changes.

---

## **📜 License**

This project is under the MIT License (MIT). See the LICENSE for more information.





