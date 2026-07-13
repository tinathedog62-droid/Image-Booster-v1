# ⚡ Image Booster V1 — Ultra-Lightweight WASM & Native Rust Imaging Workstation

Image Booster V1 is a hyper-optimized, native desktop digital signal processing (DSP) application designed for real-time pixel array manipulation and vector matrix geometry transformation. 

By utilizing **Tauri v2** as a zero-bloat system window wrapper and compiling low-level pixel crunching algorithms into **WebAssembly (WASM)** via Rust, this software bypasses standard heavy Chromium runtimes. The result is a fully self-contained production binary weighing in at an incredibly minuscule **1.2 MB** total distribution size.

---

## ✨ Engineering & Performance Metrics
* **📦 Microscopic Footprint:** ~1.2MB compiled `.exe` bundle size (over 80x smaller than comparable Electron-based media tools).
* **⚡ Bare-Metal Execution:** Image filtering algorithms bypass JavaScript overhead entirely, executing at raw machine speed inside compiled WebAssembly linear memory arrays.
* **🧠 Memory-Safe Core:** Built on Rust's strict safety standards, ensuring zero memory leaks or garbage collection spikes during high-resolution bitmap streaming.
* **🎛️ Dynamic Acoustic Layer:** Features an integrated interactive hardware synth feedback engine running on the browser's Web Audio API context.

---

## 🎨 Feature Deep-Dive

### 📐 Structural Vector Geometry Engine
* **Interactive Bounding Box:** Real-time vector cropping mechanics with precise canvas coordinate intercept hooks.
* **Aspect Scaling:** Dynamic boundary interpolation calculations allowing granular handle resizing on the corner matrices (`tl`, `tr`, `bl`, `br`).
* **Reflective Array Flipping:** Instantly applies horizontal and vertical matrix mirror reflections directly across the raw working source coordinate maps.

### 🎛️ Low-Level Linear Filter Matrix
* **Contrast Adjustments:** Granular adjustments scaling non-linearly to emphasize color variance.
* **Saturation Gradients:** Full-spectrum saturation shifts ranging from true monochrome grayscale (-100) up to hyper-vivid tone mapping (+150).
* **Brightness Thresholding:** Direct adjustments shifting the RGB luminance vectors uniformly.
* **Sharpness Convolution:** Fast image spatial frequency filtering to enhance high-contrast edges instantly.

### 🎭 Hardware Synth Feedback System
* Implements system-level browser window interaction safety compliance.
* Triggers clean acoustic sine-wave oscillators (`650Hz` dropping exponentially to `150Hz` over an exact `0.08s` decay envelope).
* Hard-capped at precisely **40% hardware gain limits** to optimize sound output for high-performance audio listening configurations without audio clipping.

### 🎨 Premium Interface Architecture
* Customized dark mode theme mapped explicitly to a sleek charcoal palette (`#1e1e24` and `#18181c`) for reduced eye strain.
* Universal system global listeners allowing immediate image asset capture via standard `Ctrl + V` OS clipboard buffers.
* Drag-and-drop file binding node interfaces.

---

## 🛠️ Project Structure & Architecture

```text
cherpify/
├── dist/                          # Static Production Asset Bundle (Target Folder)
│   ├── index.html                 # Rebuilt Dark Studio HTML Interface File
│   └── pkg/                       # Compiled WebAssembly Machine Modules
│       ├── imgboost_wasm.js       # WASM JavaScript Bridge Layer
│       └── imgboost_wasm_bg.wasm  # Binary WebAssembly Compiled Code Array
├── pkg/                           # Source WebAssembly Intermediary Modules
├── src/                           # Core Image Processor Engine (Rust)
│   └── lib.rs                     # High-Speed Multi-Threaded Filter Logic
├── src-tauri/                     # Native Desktop Shell Architecture (Tauri v2)
│   ├── capabilities/              # System-Level OS Permission Manifests
│   ├── icons/                     # Multi-Resolution Platform App Branding Assets
│   ├── src/
│   │   └── main.rs                # Windows Core Application Window Entry Point
│   ├── build.rs                   # Native Compilation Build Configuration Cargo Hook
│   ├── Cargo.toml                 # Desktop Native Dependencies Specification
│   └── tauri.conf.json            # Target Locked System Wrapper JSON Config
├── Cargo.lock                     # Strict Internal Rust Package Hash Tree
├── Cargo.toml                     # Project Main Workspace Compilation Targets
└── index.html                     # Main Frontend Workspace File Structure
