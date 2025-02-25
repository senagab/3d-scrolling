# Three.js Scroll-Based Animation

<p >
   <img src="https://img.shields.io/badge/threejs-v0.128.0-blue" alt="THREE.JS">
   <img src="https://img.shields.io/badge/GSAP-v3.12.5-yellow" alt="GSAP">
   <img src="https://img.shields.io/badge/lenis-v0.128.0-red" alt="Lenis">
</p>

A Three.js project that animates a 3D GLTF model based on user scroll input. The model rotates and floats smoothly, synchronized with the scroll progress.

## Features
- Loads and renders a `.glb` model using `GLTFLoader`
- Implements smooth scrolling animations with GSAP `ScrollTrigger`
- Adds ambient and directional lighting for improved visuals
- Applies a floating effect to the model
- Responsive and lightweight design

## Technologies Used
- [Three.js](https://threejs.org/) (v0.128.0)
- [GSAP ScrollTrigger](https://greensock.com/scrolltrigger/)
- JavaScript (ES6)
- HTML & CSS

## Installation
1. Clone the repository:
   ```sh
   git clone <your-repo-url>
   ```
2. Navigate to the project directory:
   ```sh
   cd <your-project-folder>
   ```
3. Open `index.html` in a browser or use Live Server (VSCode extension recommended).

## Usage
- Scroll up and down to see the 3D model rotate and float.
- The animation is tied to the scroll progress using GSAP `ScrollTrigger`.

## File Structure
```
📁 project-folder
│── 📄 index.html       # Main HTML file
│── 📄 script.js        # Three.js and GSAP animation logic
│── 📂 assets
│   └── 📂 models
│       └── soda_can.glb  # 3D model
│── 📂 styles
│   └── style.css      # Basic styles
```

## Issues & Fixes
- Ensure the `.glb` file path is correct (`./assets/models/soda_can.glb`).
- Avoid multiple imports of `GLTFLoader`, use the correct CDN version.
- `requestAnimationFrame` should not be canceled prematurely to maintain smooth animation.
- Proper lighting adjustments improve visibility and realism.

