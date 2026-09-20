# ⏳ Death Course: Time Manipulation Platformer

A first-person 3D obstacle course built from scratch in Unity within a strict 24-hour time limit. 

This project demonstrates rapid prototyping of core mechanics, specifically focusing on global time manipulation (slow-motion and fast-forward)[cite: 5], rigid body physics, and modular level design across distinct hazard phases[cite: 5].

---

## 🎮 Gameplay Demo

https://youtu.be/OPRp6d2IYCc


---

## ✨ Core Mechanics & Features

- **Time Manipulation System:** Players can dynamically alter the game's timescale. Pressing `[Alpha2]` triggers Slow Time to navigate tight hazard windows, while `[Alpha4]` activates Fast-Forward[cite: 5].
- **Phased Level Design:** The obstacle course is segmented into escalating difficulty tiers, including rolling boulder traps, crushing walls ("Phase Two"), and intricate laser grids ("Phase Three")[cite: 5].
- **Post-Processing Integration:** Features heavy chromatic aberration and glitch-screen effects tied to the time manipulation abilities, visually communicating the warped timescale to the player[cite: 5].
- **Custom HUD:** Minimalist on-screen UI tracks player state with dynamic resource bars at the bottom center of the screen[cite: 5].
- **Interactive Main Menu:** Fully functional start screen with a thematic background, featuring Play, Options, and Quit navigation[cite: 5].

---

## 🛠️ Tech Stack & Development

- **Engine:** Unity 3D
- **Language:** C#
- **Physics:** Unity Rigidbody System (boulders, moving platforms)
- **Rendering:** Unity Post-Processing Volume Overlays
- **Constraint:** Solo developed in exactly 24 hours.

---

## 🧠 System Architecture Highlights

### 1. Global Time Scale Controller
The time manipulation affects the physics engine globally rather than just buffing player speed. By modifying Unity's `Time.timeScale` and adjusting `Time.fixedDeltaTime` concurrently, the game smoothly transitions between slow-motion and fast-forward states without breaking physics calculations on the moving walls or boulders.

### 2. Trigger-Based UI Progression
The transition between zones (like Phase Two and Phase Three) relies on invisible trigger colliders[cite: 5]. When the player's controller intersects these bounds, the UI dynamically updates the current phase text seamlessly on the screen without interrupting gameplay[cite: 5].

### 3. Hazard Physics & Kinematics
The rolling boulders in the initial corridor utilize Unity's physics engine to maintain realistic momentum[cite: 5]. In contrast, the crushing blocks in Phase Two run on fixed logic or animation paths to ensure predictable timing for the player to utilize their time abilities[cite: 5].

---

## 🚀 Getting Started

### Prerequisites
- Unity Editor (Version 2022.3 LTS or higher recommended)
- Git

### Installation & Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/death-course-unity.git](https://github.com/your-username/death-course-unity.git)
