# TumblePop

A 2D platformer game built from scratch in C++ using the SFML library. Maneuver, vacuum up enemies, carry them around, and throw them at other enemies to clear each level — inspired by classic arcade capture-and-throw platformers.


---

## 🎮 About

TumblePop is a two-level platformer where you play as a "TumblePopper" armed with a vacuum. Suck up wandering enemies, store them, and launch them at other enemies to capture them and rack up points. Clear all enemies in Level 1 to advance to Level 2, which adds new enemy types, moving platforms, and hazards.

## ✨ Features

- **Custom physics engine** — gravity, jumping, slope collision, and platform drop-through, all built without an external physics library
- **4 enemy types** — Ghosts, Skeletons, Invisible Men, and Chelnov (a ranged enemy that throws fireballs), each with distinct movement and AI behavior
- **Capture-and-throw combat** — vacuum enemies from a distance, store multiple at once, then throw one or all of them to knock out other enemies in a chain
- **2 selectable characters** — Yellow Tumblepopper (faster movement) and Green Tumblepopper (stronger vacuum), each with different stats
- **2 levels** — hand-built Level 1, and randomized platform chunks and a slanted ramp in Level 2
- **Power-ups** — speed boost, vacuum range boost, vacuum power boost, and extra lives, spawned randomly across the level
- **Score, lives, and game over/win states**

## 🕹️ Controls

| Key | Action |
|---|---|
| Arrow Keys | Move & Jump |
| Down | Drop through platform |
| Space | Vacuum |
| Space + W/A/S/D | Aim vacuum |
| T | Throw one enemy |
| T + W/A/S/D | Aim throw (one enemy) |
| T + W/S | Snap thrown enemy up/down a platform |
| Y | Throw all stored enemies |
| Y + W/A/S/D | Aim throw (all enemies) |
| Esc | Quit game |

## 🛠️ Built With

- **Language:** C++
- **Library:** [SFML](https://www.sfml-dev.org/) (Graphics, Audio, Window)
- **IDE:** Visual Studio / Ubuntu Terminal

## 🚀 Getting Started

### Prerequisites
- [SFML](https://www.sfml-dev.org/download.php) installed and linked to the project
- Visual Studio / Ubuntu

### Running it

#### Visual Studio
1. Clone the repo:
   ```
   git clone https://github.com/your-username/Tumblepop.git
   ```
2. Open `Tumblepop.slnx` in Visual Studio.
3. Make sure SFML is correctly linked (include/lib paths and DLLs).
4. Build and run.

#### Ubuntu
1. Install the GNU G++ compiler:
   ```
   sudo apt-get install g++
   ```
2. Install SFML:
   ```
   sudo apt-get install libsfml-dev
   ```
3. Compile:
   ```
   g++ -c tumblepop.cpp
   g++ tumblepop.o -o sfml-app -lsfml-graphics -lsfml-audio -lsfml-window -lsfml-system
   ```
4. Run the game:
   ```
   ./sfml-app
   ```

> Note: the game loads assets from the `Assets/` folder at runtime, so make sure the working directory is set to the project root when running.

## 📂 Project Structure

```
Tumblepop/
├── Source.cpp          # Main game source
├── Assets/
│   ├── Backgrounds/     # Level & menu backgrounds
│   ├── Blocks/          # Tile sprites
│   ├── Font/            # UI font
│   ├── Sound/           # Music
│   └── Sprites/         # Player, enemy, and item sprites
├── Tumblepop.slnx       # Visual Studio solution
└── Tumblepop.vcxproj    # Visual Studio project file
```   
