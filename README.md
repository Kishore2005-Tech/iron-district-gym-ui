# ◈ Evasion

> **Premium Animated Product Landing Page**

[![Built With](https://img.shields.io/badge/built%20with-GSAP%20%2B%20Three.js-8B5CF6?style=flat)]()
[![Type](https://img.shields.io/badge/project-Freelance%20Client%20Work-F59E0B?style=flat)]()
[![Motion](https://img.shields.io/badge/design-Motion%20First-EC4899?style=flat)]()
[![Status](https://img.shields.io/badge/status-delivered-22C55E?style=flat)]()

---

<div align="center">

### ◈ Motion is the message. ◈
*A product landing experience where every scroll, every click, every transition is a designed moment.*

</div>

---

## 🧭 Project Overview

**Evasion** is a high-fidelity, motion-first product landing page built as a **freelance project** for a premium product brand. The entire experience is built around the principle that the journey between sections is just as important as the sections themselves.

From the first viewport to the final CTA, **nothing is static**. Every transition between pages and sections is a deliberate choreography of motion — built to make the product feel exclusive, powerful, and unforgettable.

> 💼 *Freelance project — designed, animated, and developed solo from brief to delivery.*

---

## 🌊 The Motion Experience

```
Traditional landing page:    Section 1  →  scroll  →  Section 2  (boring)

Evasion:          Scene 1 dissolves  →  camera drifts  →  Scene 2 assembles
```

Every page and section transition in Evasion is a **unique, one-of-a-kind animation sequence** — not a template, not a preset. The product moves, the typography performs, and the environment responds to the user at every step.

---

## ✦ Transition Architecture

```
╔══════════════════════════════════════════════════════════════════╗
║                    PAGE TRANSITION MAP                           ║
╠══════════════════════════════════════════════════════════════════╣
║                                                                  ║
║  HERO  ────────────────────────────────────────────────────────  ║
║   Enter  : Logo assembles from scattered particles               ║
║   Exit   : Product lifts off and pierces through the screen      ║
║                                                                  ║
║  PRODUCT SHOWCASE  ──────────────────────────────────────────── ║
║   Enter  : Scene rotates in from a 90° camera tilt               ║
║   Exit   : Product shatters into light shards → next section     ║
║                                                                  ║
║  FEATURES  ──────────────────────────────────────────────────── ║
║   Enter  : Cards drop from above in staggered sequence           ║
║   Exit   : Cards collapse inward → implode to a point of light   ║
║                                                                  ║
║  STORY / ABOUT  ────────────────────────────────────────────── ║
║   Enter  : Text materializes word by word through noise shader   ║
║   Exit   : Environment fades into deep void → warp tunnel        ║
║                                                                  ║
║  TESTIMONIALS  ─────────────────────────────────────────────── ║
║   Enter  : Quotes orbit in from 3D carousel depth                ║
║   Exit   : Quotes spiral and dissolve into next scene            ║
║                                                                  ║
║  CTA / FOOTER  ─────────────────────────────────────────────── ║
║   Enter  : Scene erupts from below like a stage reveal           ║
║   Idle   : Ambient floating particles, cursor-reactive glow      ║
║                                                                  ║
╚══════════════════════════════════════════════════════════════════╝
```

---

## ✨ Feature Highlights

### 🎬 Animation System
- **Scroll-driven scene control** — scroll position directly drives animation progress
- **Custom transition timelines** — each section has its own named GSAP timeline
- **Bidirectional animations** — scroll back and every animation reverses perfectly
- **Cursor-reactive environment** — 3D elements tilt and glow in response to mouse position
- **Kinetic typography** — text doesn't appear, it *performs*
- **Shader-based effects** — distortion, glow, noise, and chromatic aberration via GLSL

### 🖼️ Visual Design
- **Dark luxury aesthetic** — deep blacks, neon accents, premium feel
- **3D product visualization** — interactive product model with ambient rotation
- **Floating particle atmosphere** — persistent ambient particles throughout experience
- **Dynamic lighting** — light sources shift based on scroll position and cursor
- **Glass morphism UI panels** — frosted depth on all UI overlays
- **Fluid mesh backgrounds** — procedurally animated background geometry

### ⚡ Interaction Design
- **Magnetic buttons** — CTA elements pull toward the cursor within proximity
- **Spring physics** — all interactive elements use physics-based easing
- **Hover depth effects** — cards and panels push into Z-axis on hover
- **Custom animated cursor** — brand cursor with trail and click burst effects
- **Smooth scroll inertia** — native scroll replaced with momentum-based scrolling

---

## 🛠️ Tech Stack

```
Animation Engine    →  GSAP 3 (GreenSock) + ScrollTrigger + CustomEase
3D Rendering        →  Three.js (WebGL)
Shaders             →  GLSL (custom vertex & fragment shaders)
Smooth Scroll       →  Lenis (smooth scroll inertia)
Framework           →  Next.js / React
Styling             →  Tailwind CSS + CSS custom properties
3D Models           →  Blender → glTF / GLB (Draco compressed)
Post-Processing     →  Three.js EffectComposer
                        — UnrealBloomPass
                        — ChromaticAberrationEffect
                        — DepthOfFieldEffect
Fonts               →  Variable fonts with optical sizing
Deployment          →  Vercel
```

---

## 📁 Project Structure

```
evasion/
├── app/
│   ├── page.jsx                    # Entry point — orchestrates all sections
│   └── layout.jsx                  # Global cursor, smooth scroll, loader
├── components/
│   ├── sections/
│   │   ├── Hero.jsx                # Hero scene + particle logo intro
│   │   ├── ProductShowcase.jsx     # 3D interactive product model
│   │   ├── Features.jsx            # Staggered feature cards
│   │   ├── Story.jsx               # Brand narrative section
│   │   ├── Testimonials.jsx        # 3D carousel quotes
│   │   └── CTA.jsx                 # Final conversion section
│   ├── canvas/
│   │   ├── SceneManager.jsx        # Global Three.js scene controller
│   │   ├── ProductModel.jsx        # 3D product renderer
│   │   ├── ParticleSystem.jsx      # Ambient & transition particles
│   │   └── PostProcessing.jsx      # Bloom, aberration, DOF pipeline
│   ├── transitions/
│   │   ├── TransitionEngine.jsx    # Master transition orchestrator
│   │   ├── timelines/              # Per-section named GSAP timelines
│   │   │   ├── hero.timeline.js
│   │   │   ├── showcase.timeline.js
│   │   │   ├── features.timeline.js
│   │   │   └── cta.timeline.js
│   │   └── useScrollTimeline.js    # Scroll → animation sync hook
│   └── ui/
│       ├── Cursor.jsx              # Custom branded cursor
│       ├── Loader.jsx              # Intro preloader animation
│       ├── MagneticButton.jsx      # Physics-based CTA buttons
│       └── Navbar.jsx              # Animated navigation
├── shaders/
│   ├── particle.vert               # Particle vertex shader
│   ├── distortion.frag             # Mesh distortion fragment shader
│   ├── noise.glsl                  # Simplex/Perlin noise utilities
│   └── glow.frag                   # Bloom glow shader
├── lib/
│   ├── gsap.config.js              # GSAP plugin registration
│   ├── lenis.config.js             # Smooth scroll setup
│   └── three.utils.js              # Scene helpers and loaders
├── public/
│   └── models/                     # Compressed .glb product assets
└── README.md
```

---

## ⚙️ Getting Started

### Prerequisites

- Node.js `v18+`
- Browser with **WebGL 2.0** + hardware acceleration enabled

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/evasion.git
cd evasion

# 2. Install dependencies
npm install

# 3. Start development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000)

> ⚠️ **For the full experience: use desktop Chrome or Firefox with GPU acceleration on.**
> Mobile degrades gracefully but the full motion system is desktop-optimized.

---

## ⚡ Performance Strategy

High-motion WebGL experiences can be expensive. Evasion was engineered to stay smooth:

| Optimization | Implementation |
|---|---|
| 3D Model Compression | Draco GLTF — up to 90% size reduction |
| Texture Optimization | Compressed KTX2 textures via Basis transcoder |
| Render Budget | Scene complexity scales with device GPU tier |
| Animation Loop | Single centralized `rAF` loop — no conflicts |
| Code Splitting | Three.js and GSAP loaded only when viewport ready |
| Preloading | Next section assets preloaded during active transition |
| Reduced Motion | Full `prefers-reduced-motion` support — no accessibility compromise |

**Target:** 60fps on mid-range desktop hardware, smooth degradation on lower-tier devices.

---

## 🎨 Design Language

**Evasion's visual identity is built on three pillars:**

```
DEPTH        →  Everything exists in 3D space. Flat is forbidden.
RESTRAINT    →  Premium feel comes from what you don't show, not what you do.
INTENT       →  Every animation earns its place. Nothing moves without reason.
```

**Color system:**
```
Background   →  #050508  (near-black with cool undertone)
Primary      →  #E0E0FF  (off-white with blue tint)
Accent 1     →  #7C3AED  (deep violet — power, exclusivity)
Accent 2     →  #06B6D4  (electric cyan — energy, precision)
Glow         →  rgba(124, 58, 237, 0.4)  (bloom halo)
```

---

## 💼 Freelance Project Details

| | |
|---|---|
| **Client Type** | Premium product brand |
| **My Role** | Solo — UI/UX Design + Frontend Development + Animation |
| **Deliverables** | Full source code, live deployment, asset library, client handoff docs |
| **Scope** | End-to-end — from brief and wireframes to final deployed product |
| **What this demonstrates** | Motion design, 3D web, custom shader work, scroll storytelling, performance optimization |

---

## 📸 Preview

> *(Replace with actual recordings)*

```
/docs/preview/hero-intro.gif           ← Particle logo assembly
/docs/preview/product-showcase.gif     ← 3D product interaction
/docs/preview/section-transitions.gif  ← Full transition sequence
/docs/preview/cursor-interaction.gif   ← Magnetic cursor demo
```

🔗 **Live Demo:** [evasion.vercel.app](https://evasion.vercel.app)

---

## 📄 License

Shared for **portfolio and reference purposes only.**
Client brand assets, product models, and proprietary content are excluded from this repository.
Not licensed for reuse, resale, or redistribution.

---

## 👤 Designer & Developer

**Kishore** — UI/UX Designer · Frontend Developer · Motion Engineer
[GitHub](https://github.com/your-username) · [LinkedIn](https://linkedin.com/in/your-profile) · [Portfolio](https://your-portfolio.com)

---

<div align="center">

**◈ Evasion** — *Where product meets performance meets poetry.*

Designed and developed with obsessive precision. ✦

</div>
