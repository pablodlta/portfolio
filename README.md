# Pablo de la Torre Aragón — Industrial Design & Product Development Engineering Portfolio

> **Industrial Design & Product Development Engineering Portfolio**  
> *Undergraduate at Universidad de Cádiz, Escuela Superior de Ingeniería*  
> *Specializing in Advanced 3D CAD Surfacing, DFM Tooling, Eco-Design LCA, and AI-Driven CAD Synthesis.*

---

## 🌟 Executive Summary & Engineering Architecture

This repository contains the production web portfolio of **Pablo de la Torre Aragón**, engineered according to high-standard Hardware Product Design and Design Technologist hiring criteria (e.g., Google Hardware / Nest / Pixel).

The portfolio presents end-to-end hardware deliverables: parametric 3D CAD surfaces, exploded electro-mechanical assemblies, 2D technical orthographics (ISO / DIN standards), Color Material Finish (CMF) matrices, Ashby material selection charts, physical FDM functional prototypes, and interactive 3D WebGL assets.

---

## 🚀 Key Highlights & Projects

### 1. Automated CAD Synthesis via KBE & Local LLM (Bachelor's Thesis, 2026–Present)
* **Academic Affiliation:** Bachelor's Thesis (TFG) & Curricular Practices (12 ECTS) at **GOAL Lab** ([TIC-259](https://tic259.uca.es/)), Escuela Superior de Ingeniería (ESI), Universidad de Cádiz.
* **Tooling:** SolidWorks COM API (`win32com`), Python 3.12, Model Context Protocol (MCP), Local LLM (Ollama / DeepSeek).
* **Architecture:** Translates mechanical design intent in natural language into strictly validated JSON AST schemas, enforces ISO clearance/draft rules via an MCP server, and generates native parametric SolidWorks parts with editable FeatureManager history trees.
* **Validation:** Sub-3.2s inference and 100% rebuildable parametric topology.

### 2. Koky: Luxury Pet Care Dispenser (May 2025)
* **Tooling & Process:** SolidWorks Surfacing, Deep Drawing, Impact Extrusion, CNC Turning, FDM Functional Prototyping.
* **Features:** Impact-resistant deep-drawn aluminum bottle with bi-directional helical grip sweeps, threadless friction-fit retention ring, separable PP dispenser core for circular recycling, and secondary packaging compliant with ISO 3394 palletization (84 units/layer).
* **Interactive 3D:** Integrated Google `<model-viewer>` 3D WebGL interactive inspection with floating CMF callouts.

### 3. AeroStream: Modular Eco-Blender System (2026)
* **Tooling & Process:** High-Pressure Die Casting (Al 6061-T6), Injection Stretch Blow Molding (ISBM - Tritan™ Renew), PEEK Gear Injection, PVD Diamond-Like Carbon (DLC) coating (>2500 HV).
* **Features:** 110 mm vertical handle clearance accommodating P95 male metacarpals, 1.5-turn twist-and-lock safety interlock, reversible M4 DFD fasteners, and 100% plastic-free folding packaging.
* **Validation:** 13 ISO/DIN technical orthographic sheets and SolidWorks Sustainability LCA demonstrating a 42% lifecycle carbon mitigation.

### 4. UCAchew: Biomechanical Canine Toy & Ashby Selection (2025)
* **Tooling & Process:** Ashby Multi-Objective Screening (CES EduPack), Extrusion Blow Molding with split dies.
* **Features:** Replaced hazardous nylon and degradable rubber with Aliphatic Ether TPU (Shore A80) with 45 MPa tensile strength and >85 kN/m tear propagation resistance. Features a uniform 5.0 mm wall hollow cavity for damping canine jaw impacts (235–328 PSI).
* **Compliance:** European Standard EN 71-3 (heavy-metal migration) and FDA 21 CFR §177.2600.

### 5. Modular Flat-Pack Divider & Telework System (Nov 2025)
* **Tooling & Process:** CATIA V5, SolidWorks, 6063-T6 Aluminum Hot Extrusion, 5-Axis CNC Router Plywood Milling.
* **Features:** Integrated dual-function aluminum hinge profile with continuous 360° stainless steel axial pins, CNC keyhole matrices for drop-and-lock cantilever desks (63° brace), and a 5-layer zero-slack corrugated master carton fitting standard EPAL 1 pallets.
* **Validation:** 1:1 user testing, domestic ergonomic focus groups, and ISO engineering orthographics.

---

## 🛠️ Frontend Engineering & Accessibility Standards

The web architecture was refactored to eliminate technical debt and comply with **WCAG 2.1 AA standards**:
* **Ahead-Of-Time (AOT) Compiled CSS:** Replaced runtime Tailwind CDN scripts with a compiled, purged, and minified stylesheet (`assets/css/dist.min.css`, ~34 KB), eliminating Cumulative Layout Shift (CLS) and optimizing First Contentful Paint (FCP).
* **Native Accessible Dialogs:** Custom div modals replaced with native HTML5 `<dialog>` elements utilizing `.showModal()`, focus trapping, focus restoration to trigger elements, light dismiss (backdrop click), and standard keyboard `Escape` capture.
* **WCAG 2.1 AA Contrast:** All text, badges, and metadata strictly exceed the 4.5:1 contrast minimum on light backgrounds (slate-600/slate-700 on slate-50).
* **Touch Target Sizing:** All interactive buttons and navigation links guarantee touch targets $\ge 48 \times 48\text{ px}$.
* **Motion Sensitivity:** Integrated `prefers-reduced-motion` media queries disabling vestibular animations.
* **Semantic Data Sheets:** Engineering specifications structured using `<dl>`, `<dt>`, and `<dd>` description lists.

---

## 💻 Local Development & Build

### Prerequisites
* [Node.js](https://nodejs.org/) (v18+)
* [npm](https://www.npmjs.com/)

### Build Commands
```bash
# Install dependencies
npm install

# Compile minified production CSS (AOT)
npm run build:css

# Watch for changes during development
npm run watch:css
```

---

## 📬 Contact & Portfolio Links

* **Author:** Pablo de la Torre Aragón
* **LinkedIn:** [linkedin.com/in/pablodlta](https://www.linkedin.com/in/pablodlta/)
* **Email:** [pablodelatorrearagon@gmail.com](mailto:pablodelatorrearagon@gmail.com)
* **Portfolio Repository:** [github.com/pablodlta/portfolio](https://github.com/pablodlta/portfolio)