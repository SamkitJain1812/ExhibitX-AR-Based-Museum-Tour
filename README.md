<div align="center">

# 🏛️ ExhibitX — Step Inside History

### *An immersive AR platform that brings 5,000 years of human civilisation into your physical space*

[![Built with React](https://img.shields.io/badge/Built%20with-React-61DAFB?logo=react)](https://reactjs.org/)
[![AR.js](https://img.shields.io/badge/AR-AR.js-orange)](https://ar-js-org.github.io/AR.js-Docs/)
[![Three.js](https://img.shields.io/badge/3D-Three.js-black?logo=three.js)](https://threejs.org/)

<br/>

> *"History is no longer behind glass."*

</div>

---

## 📖 About the Project

Traditional museums fail modern audiences in three critical ways:

- 🔒 **Engagement Gap** — Static glass displays don't compete with the interactive digital experiences younger audiences expect
- 🔍 **Physical Limitation** — Artifacts behind barriers prevent understanding of true scale, texture, and architectural detail
- ✈️ **Accessibility Barrier** — The world's greatest heritage is geographically locked — most people will never travel to these monuments

**ExhibitX** solves all three. It is a **web-based Augmented Reality museum platform** that places high-quality 3D models of historical monuments directly into the user's real-world environment — in their bedroom, classroom, or backyard — using just a smartphone browser.

No app download. No AR headset. No travel. Just open a link and step inside history.


---

## ✨ Key Features

| Feature | Description |
|---|---|
| 📦 **Interactive 3D Inspection** | Rotate, scale, and zoom into monuments with high-res PBR textures revealing fine architectural details |
| 📡 **GPS Geo-Anchored AR** | Live GPS + compass tracking — monuments placed 8m ahead and shift in real space as you walk and turn |
| 🪟 **AR Portal Environments** | Step through virtual doorways into 360° reconstructions of a monument's original historical environment |
| ℹ️ **Floating Info Panel** | Contextual history panel (era, builder, height, UNESCO status) floats in AR — always readable |
| 🎮 **Gamified Restoration** | Repair fractured digital artifacts using AR gestures — learning through interaction |
| 🌐 **Zero Install** | Runs entirely in any camera-enabled smartphone browser via AR.js — no app store needed |

---

## 🗺️ Monument Collections

### Indian Heritage *(Primary Focus)*
- Taj Mahal · Agra
- Qutub Minar · New Delhi
- Red Fort · Old Delhi
- Konark Sun Temple · Odisha

### Egyptian Wonders
- Great Pyramid of Giza
- Great Sphinx · Giza
- Luxor Temple · Thebes
- Abu Simbel · Aswan

### Roman Grandeur
- The Colosseum · Rome
- The Pantheon · Rome
- Roman Forum · Rome
- Arch of Constantine · Rome

---

## 🛠️ Tech Stack

| Layer | Technology | Purpose |
|---|---|---|
| ⚛️ **Frontend** | React.js + Vite | Component-based UI, routing, state management |
| 🔷 **3D Engine** | Three.js / React Three Fiber | PBR-textured 3D monument rendering |
| 📡 **Augmented Reality** | AR.js + A-Frame | GPS geo-anchored AR — cross-platform, browser-native |
| 🗺️ **Geolocation** | Navigator Geolocation API | Live `watchPosition()` coordinate streaming |
| 🧭 **Compass** | DeviceOrientation Event API | Real-time compass heading for directional AR |
| 🎨 **Styling** | CSS + Tailwind CSS | Historical gold-and-parchment responsive UI |
| 📦 **Models** | GLTF / GLB | Lightweight, web-optimised 3D monument assets |

---

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

```bash
node -v      # Node.js v18 or higher
npm -v       # npm v9 or higher
```

> Download Node.js from [nodejs.org](https://nodejs.org/) if not installed.

---

### 📥 Clone the Repository

```bash
git clone https://github.com/SamkitJain1812/AR-Based-Museum-Tour_Fosshack-26.git
```

```bash
cd AR-Based-Museum-Tour_Fosshack-26
```

---

### 📦 Install Dependencies

```bash
cd my-react-app
```

```bash
npm install
```

---

### ▶️ Run Locally

```bash
npm run dev
```

The app will start at:

```
http://localhost:5173
```

Open it in your browser. For the AR features, open it on a **mobile device** using your local network IP (e.g. `http://192.168.x.x:5173`) and allow camera + location permissions when prompted.

---

### 🏗️ Build for Production

```bash
npm run build
```

```bash
npm run preview
```

---

## 📁 Project Structure

```
AR-Based-Museum-Tour/
│
├── Frontend/                  # Static HTML dashboard version
│
├── Models/                    # 3D model assets (.glb / .gltf)
│
├── my-react-app/              # Main React + Vite application
│   ├── src/
│   │   ├── Aframe.jsx         # AR.js + A-Frame AR scene wrapper
│   │   ├── App.jsx            # Root app component & routing
│   │   ├── Firstpage.jsx      # Landing / intro screen
│   │   ├── Maindashbord.jsx   # Main dashboard (world selector)
│   │   ├── Egypt.jsx          # Egyptian Wonders section
│   │   ├── Rome.jsx           # Roman Grandeur section
│   │   ├── Romeexplore.jsx    # Rome AR explore view
│   │   ├── Tajmahalexplore.jsx # Taj Mahal AR experience
│   │   ├── KonarkTemple.jsx   # Konark Sun Temple component
│   │   ├── Qutub.jsx          # Qutub Minar component
│   │   ├── RedFort.jsx        # Red Fort component
│   │   ├── Luxor.jsx          # Luxor Temple component
│   │   ├── Pantheon.jsx       # The Pantheon component
│   │   ├── Simbel.jsx         # Abu Simbel component
│   │   ├── Sphinx.jsx         # Great Sphinx component
│   │   ├── Arc of Constantine # Arch of Constantine component
│   │   ├── MainDashbord.CSS   # Dashboard styles
│   │   ├── Rome.css           # Rome section styles
│   │   ├── Qutub.css          # Qutub section styles
│   │   ├── First.css          # Landing page styles
│   │   └── main.jsx           # React entry point
│   │
│   ├── index.html             # App HTML shell
│   ├── package.json           # Dependencies
│   ├── vite.config.js         # Vite configuration
│   └── eslint.config.js       # ESLint configuration
│
├── LICENSE
└── README.md
```

---

## 💡 Unique Selling Points (USP)

**1. Truly Zero-Barrier Access**
Unlike native AR apps (Apple ARKit, Google ARCore), ExhibitX runs in any modern browser. A student in a remote village with a basic Android phone gets the same experience as someone with an iPhone 15.

**2. GPS Movement-Aware AR**
Most web AR solutions place models on flat surfaces. ExhibitX uses live GPS `watchPosition()` + DeviceOrientationEvent to anchor monuments geographically — walk around them like they're actually there.

**3. India-First Focus**
ExhibitX is built to promote Indian cultural heritage to the world, while making it accessible to every Indian student regardless of geography or economic background.

**4. Open Source**
Fully open source under Apache- 2.0 license. Any museum, school, or cultural organisation can fork and deploy their own instance.

**5. Education + Gamification**
The gamified restoration module turns passive museum browsing into active learning — students *repair* artifacts, not just view them.

---

## 🌍 Social Impact

- 🏫 **Students** get virtual field trips to monuments they'll never physically visit
- ♿ **Accessible** to anyone with a camera-enabled smartphone — no economic barrier
- 🏺 **Preservation** — 3D documentation protects heritage against time and disaster
- 🇮🇳 **Tourism** — promotes Indian monuments to a global digital audience

---

## 👥 Team ExhibitX

- Samkit Jain
- Sonu Jha
- Amogh Raj
- Monu Jha

---

<div align="center">

**ExhibitX** · FossHack 2026 · Made with ❤️ for India

*"Step inside. The history is waiting."* 🏛️✨

</div>
