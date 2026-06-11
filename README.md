# 🧠 NEOSYNAPSE

### Bio-Adaptive Interface for Cognitive Urban Environments

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://your-username.github.io/neosynapse)
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

**[Click here to run the simulation](https://your-username.github.io/neosynapse)**

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
git clone https://github.com/your-username/neosynapse.git
cd neosynapse
