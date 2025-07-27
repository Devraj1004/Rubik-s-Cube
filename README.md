# 🧠 Rubik's Cube Solver and Visualizer

## 🚀 Overview

This project is a complete **2D Rubik's Cube Simulator and Solver** built using **Python and Pygame**, designed for the **AeroHack Design Challenge** hosted by **Collins Aerospace**.

It features:
- A visually accurate unfolded cube layout
- Full keyboard-controlled face rotations
- Scrambling, resetting, and auto-solving functionality
- Integration with **Kociemba’s Optimal Solver Algorithm**
- Smooth animated transitions for each move
- Optional fallback BFS solver for unsupported patterns

---

## 🧩 Features

| Feature                  | Description |
|--------------------------|-------------|
| 🎮 Interactive UI        | Rotate any face using keyboard (F, R, U, L, D, B + Shift) |
| 🌀 Animated Solving       | Solver visually animates each move |
| 🧠 Dual Solver Engines   | Kociemba’s algorithm + BFS fallback |
| 🎲 Scramble Button       | Press `S` to randomize the cube |
| 🔄 Reset Button          | Return to solved state using `SPACE` |
| ⌨️ Clean Controls Help   | On-screen, color-coded instructions |
| 🧱 Custom Cubelets        | Each face built using a clear color-coded 3x3 grid |

---

## 🛠️ Tech Stack

- **Language:** Python 3.11+
- **Graphics:** Pygame (2D cube layout)
- **Solving Algorithms:**
  - `Kociemba` (optimal, advanced)
  - `BFS` (guaranteed fallback)
- **Build Tools:** MSVC v143 + Windows SDK (for kociemba)

---

## 🎮 Controls
Rotations:
  F / Shift+F → Front (clockwise / counter-clockwise)
  R / Shift+R → Right
  U / Shift+U → Up
  L / Shift+L → Left
  D / Shift+D → Down
  B / Shift+B → Back

Other:
  S        → Scramble
  SPACE    → Reset to solved
  M        → Solve using AI
  ESC      → Quit

---

## 🔧 Installation (Step-by-Step Guide)

Follow these instructions to run the Rubik’s Cube Visualizer + Solver on your Windows system.

---

### ✅ 1. Clone this Project

If you have Git installed, open **Command Prompt** or **Git Bash** and run:

```bash
git clone https://github.com/Devraj1004/Rubik-s-Cube.git
cd Rubik-s-Cube
```

> 🔸 This downloads the code to your computer and opens the project folder.

---

### ✅ 2. Create a Virtual Environment (Recommended)

This helps keep the project’s Python libraries separate from your system-wide Python.

```bash
python -m venv .venv
```

Then activate it:

```bash
.venv\Scripts\activate
```

> ⚠️ If this shows an error, make sure you have Python 3.10 or later installed and added to your system PATH.

---

### ✅ 3. Install Required Libraries

Install the packages needed to run the project:

```bash
pip install -r requirements.txt
```

This will install:

* `pygame` → for the cube's user interface
* `kociemba` → the AI solver (optional but recommended)

---

### ✅ 4. (Optional but Recommended) Install Kociemba Solver

If you want to use the **fast optimal solver**, install Kociemba:

```bash
pip install kociemba
```

> 💡 **Note:** If it fails, you’ll need to install **C++ Build Tools** (MSVC v143) and **Windows 10/11 SDK**. You can get them from here:
> 👉 [Visual C++ Build Tools Download](https://visualstudio.microsoft.com/visual-cpp-build-tools/)

---

### ✅ 5. Run the Application

Once everything is set up, just run:

```bash
python rubix.py
```

(or whatever your main script filename is)

🎉 You should see the 2D Rubik’s Cube window open!

---

### 🧩 Having Issues?

* Make sure you activated the virtual environment
* Use Python 3.10+ (Python 3.11+ preferred)
* If `kociemba` fails to install, run without it — the app still works with the fallback solver!

---

## 🖼 Screenshots
- Initial State:
  
  <img width="863" height="387" alt="image" src="https://github.com/user-attachments/assets/7eb57820-b53b-49af-85d9-a4171b07e9fe" />
  
- Scrambled Cube:
  
  <img width="863" height="380" alt="image" src="https://github.com/user-attachments/assets/d1b602fc-3a30-4253-b908-29a00c3bfa0b" />
  
- Magic Solver (Auto solves the Cube):
  
  <img width="863" height="376" alt="image" src="https://github.com/user-attachments/assets/102f8cfb-c1d2-4d1d-afed-4bcdc28c66d5" />
  
- Goal State Reached:
  
  <img width="865" height="380" alt="image" src="https://github.com/user-attachments/assets/8060af24-8fd9-4d3a-bb73-842ef6eee267" />

---

## 🙌 Acknowledgements

Kociemba's Algorithm - for optimal Rubik’s Cube solutions

Collins Aerospace - for the AeroHack Challenge platform
