# 3D Agency

3D Agency is a scroll-driven product showcase for a modern coffee brand. It combines editorial product copy, procedural Three.js models, animated section transitions, and lightweight storefront interactions into a SPA experience.

## Overview

The page presents three coffee-focused products as interactive 3D objects:

- **Artisanal Bean Bag**: a kraft paper whole-bean bag with folded panels, gussets, valve details, and label accents inspired by jasmine, bergamot, and honey tasting notes.
- **To-Go Cup**: a tapered lidded cup with visible espresso and micro-foam layers, plus a ribbed cardboard insulation sleeve.
- **House Mug**: a heavy stoneware mug with a hand-thrown profile, warm matte glaze, clay speckles, a thick handle, coffee surface, and foot ring.

As the user scrolls, GSAP ScrollTrigger moves each product into view while Three.js keeps the scene alive with soft idle motion, warm lighting, and transparent canvas rendering over the page layout.

## Features

- Scroll-based 3D product choreography.
- Procedural Three.js product models with custom materials and canvas textures.
- Coffee-themed editorial sections and product cards.
- Add-to-cart buttons that update the visible cart quantity.
- Bottom-right music toggle for `Corner_Booth_View.mp3`.
- Responsive layout using Tailwind utility classes.
- Warm cafe-inspired visual direction with kraft paper, ceramic glaze, espresso, cream, and amber tones.

## Stylistic Changes

- Replaced simple placeholder shapes with more descriptive procedural product models.
- Added tactile surface details such as paper speckles, ribbed cardboard, layered drink bands, matte ceramic glaze, and clay speckles.
- Tuned the product forms to match their descriptions instead of reading as generic primitives.
- Added subtle tasting-note cues to the bean bag label using simple 3D accents.
- Kept the visual language clean, modern, and product-focused rather than decorative.

## Technical Changes

- Built as a Vite project with a single `index.html` entry point.
- Uses CDN-loaded Three.js, GSAP, ScrollTrigger, and Tailwind browser utilities.
- Preserves the main product objects as `productBag`, `productCup`, and `productMug` so the scroll timeline can animate them consistently.
- Adds small helper functions for reusable rounded geometry, label panels, speckled materials, accent dots, and shadow setup.
- Tracks cart state in the inline script and updates the header cart display after each product click.
- Adds guarded audio play/pause logic to avoid console errors from missing elements or browser autoplay restrictions.

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