# 🧠 NEOSYNAPSE

### Bio-Adaptive Interface for Cognitive Urban Environments

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://khan34535-sudo.github.io/NEOSYNAPSE-/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

---

## 🚨 What is NEOSYNAPSE?

**NEOSYNAPSE** is the world's first smartwatch simulation that combines:

| Feature | Description |
|:---|:---|
| 🧘 **Cognitive Mode Toggle** | UI auto-simplifies when stress is detected (cool colors, larger calming typography) |
| 🗺️ **Walking Navigation** | Step-by-step directions to nearest cooling station with live ETA and progress bar |
| 🚁 **Thermal Rescue Dispatch** | Automatically dispatches a rescue pod when heat stress becomes critical (48°C + HRV collapse) |
| 📍 **Live GPS Tracking** | Real-time coordinates for both pedestrian and emergency vehicle |

> **No one has packaged this together. NEOSYNAPSE closes the loop between bio-signals, adaptive UI, and city infrastructure.**

---

## 🎯 Why This Exists

Most smartwatches today:
- ❌ Add to cognitive load when you're already stressed
- ❌ Don't adapt their interface to your mental state
- ❌ Can't automatically dispatch help when walking is unsafe

NEOSYNAPSE solves all three.

---

## 🖥️ Live Demo

**[Click here to run the simulation](https://khan34535-sudo.github.io/NEOSYNAPSE-/)**

---

## 📸 Preview

| Normal Mode | Emergency Mode |
|:---:|:---:|
| ![Normal Demo](demo/demo-preview.png) | Walking navigation + cooling station routing |

---

## 🏗️ Features Demonstrated

### Normal Circumstance
- Real-time GPS coordinates (user + cooling station)
- Walking ETA based on 4.2 km/h average speed
- Progress bar showing journey completion
- Step-by-step navigation with landmarks
- "Start / Add stop / Share" actions

### Emergency Circumstance (Automatic)
- Triggers when: Heat Index > 45°C + HRV < 30ms + Distance to cooling > 10 min
- Rescue pod dispatched automatically
- Live GPS tracking of rescue vehicle
- ETA countdown + distance remaining
- Driver notification interface
- "Do NOT walk" intervention

### Cognitive Mode
- Manual toggle OR auto-trigger on stress
- Shifts to cool blue/green color palette
- Reduces visual density (fewer metrics)
- Enlarges and lightens typography

---

## 🛠️ Tech Stack

| Layer | Technology |
|:---|:---|
| Frontend | HTML5, CSS3, JavaScript (Vanilla) |
| Styling | Glassmorphism, Flexbox, CSS Animations |
| Geolocation | Simulated GPS (extensible to real API) |
| State Management | Pure JS |
| Deployment | GitHub Pages |

---

## 🚀 Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/khan34535-sudo/NEOSYNAPSE-.git
cd NEOSYNAPSE-
open index.html
# or use Live Server in VS Code
NEOSYNAPSE-/
├── index.html          # Main simulation (two watches)
├── README.md           # This file
├── LICENSE             # MIT License
├── CONTRIBUTING.md     # Contribution guidelines
└── demo/
    └── demo-preview.png # Screenshot for README
// Use browser geolocation API
navigator.geolocation.getCurrentPosition((position) => {
    userLat = position.coords.latitude;
    userLng = position.coords.longitude;
});
// Pseudocode for future integration
wearableAPI.onHeartRateChange((hrv) => {
    if (hrv < 30 && heatIndex > 45) {
        triggerEmergencyDispatch();
    }
});
// API call to dispatch rescue pod
fetch('https://api.neom-mobility.com/v1/dispatch', {
    method: 'POST',
    body: JSON.stringify({ userId, gps, priority: 'critical' })
});

---

## Instructions

1. **Select all** the text inside the code block above
2. **Copy** (Ctrl+C or Cmd+C)
3. **Go to** your GitHub repository: `https://github.com/khan34535-sudo/NEOSYNAPSE-`
4. **Click** on `README.md`
5. **Click** the pencil icon (Edit)
6. **Paste** (Ctrl+V or Cmd+V) — replace everything
7. **Scroll down** and click **"Commit changes"**

Done.
