# ⛏️ Manic Miner (1983) — ZX Spectrum 48K HTML5 Edition

A faithful, standalone, zero-dependency browser recreation of **Matthew Smith's 1983 platforming masterpiece *Manic Miner*** (originally published by Bug-Byte Software Ltd.), powered by the [SkoolKit Manic Miner Disassembly](https://skoolkit.ca/disassemblies/manic_miner/).

Runs directly in any modern desktop or mobile browser — no plugins, build steps, or external assets required.

---

## 🎮 Play Online / Local

- **Direct Play**: Double-click [`index.html`](file:///c:/Users/ross/Documents/Projects/manic/index.html) or [`ManicMiner.html`](file:///c:/Users/ross/Documents/Projects/manic/ManicMiner.html) in your browser.
- **GitHub Pages**: Automatically playable when deployed from the `main` branch (at `https://rosstinnion.github.io/Games/` or `https://rosstinnion.github.io/Games/ManicMiner.html`).

---

## ✨ Features

### 🕹️ Authentic 1983 ZX Spectrum Engine
- **Self-Contained 48K RAM**: The entire original `.z80` snapshot (49,152 bytes) is embedded directly into the code and initialized in memory on boot.
- **1-Bit Web Audio Beeper Synthesizer**: Cycle-accurate pitch emulation for *In the Hall of the Mountain King* (in-game music) and *The Blue Danube* (title piano sequence).
- **50Hz ULA Display & CRT Shader**: Authentic 256×192 pixel display with 32×24 attribute color cells, border emulation, flashing attributes, and toggleable CRT scanlines.

### 🚀 Modern Enhancements
- **Strict 4:3 Fullscreen Display**: Automatically maintains authentic 4:3 proportions centered with pillarbox/letterbox bars on widescreen and ultrawide monitors (double-click canvas or press **⛶ Fullscreen**).
- **💾 5-Slot Save State Manager**:
  - **Quick Save (`F5`)** and **Quick Load (`F9`)** hotkeys.
  - Interactive UI with visual screen thumbnails, cavern name, score, lives, and timestamps.
  - Persistent storage in browser `localStorage`.
  - **JSON Export & Import** for backup and sharing states across devices.
- **⏪ Death-Save Time Rewind**:
  - Automatically freezes time on fatal hits (hazards, guardians, fall heights).
  - Hold **Left (`←` / `Q`)**, **Backspace**, or **`[`** while in death pause to smoothly rewind time backward frame-by-frame away from the hazard without moving your hands across the keyboard.
  - Releasing the key resumes normal gameplay at the safe point.
- **⚡ Accelerated Cavern Completion**:
  - Fast, punchy air-bar countdown (~1.1 seconds for a full bar) with ascending score pitch sweeps.
  - Hold any action key (`Space`, `Enter`, arrows) to turbo-skip in ~0.3 seconds.
- **🛠️ Built-in Trainers & Cheats**:
  - Original authentic **6031769** boot teleporter (toggleable or typeable in-game).
  - 20-Cavern warp grid.
  - Infinite Lives, Infinite Air, and Invincibility toggles.
  - Instant item collector and cavern portal unlocker.
- **📱 Touch & Mobile Controls**: On-screen buttons with full touch hold support for mobile and tablet play.
- **📂 Custom `.z80` Loader**: Optional file picker to test or load alternative `.z80` ROMs or hacks.

---

## ⌨️ Controls

| Action | Primary Keyboard | Secondary / Spectrum | Touch Controls |
| :--- | :--- | :--- | :--- |
| **Move Left** | `←` Arrow | `Q`, `E`, `T`, `U`, `O`, `5` | `◀ LEFT` |
| **Move Right** | `→` Arrow | `W`, `R`, `Y`, `I`, `P`, `8` | `RIGHT ▶` |
| **Jump** | `Space` / `↑` Arrow | `Z`, `X`, `C`, `V`, `B`, `N`, `M`, `0`, `7` | `▲ JUMP` |
| **Rewind in Death Pause** | **Hold `←` Left Arrow** | Hold `Q`, `Backspace`, `[` | Hold `◀ LEFT` / `⏪ REW` |
| **Rewind Time (Live)** | Hold `Backspace` | Hold `[` | Hold `⏪ REW` |
| **Instant -2s Rewind** | `Delete` | `]` | — |
| **Quick Save State** | `F5` | — | Click `💾` |
| **Quick Load State** | `F9` | — | Click `📂` |
| **Start Game** | `Enter` | `NumpadEnter` | `ENTER` |
| **Pause / Resume** | `A`, `S`, `D`, `F`, `G` | — | `⏸ Pause` button |
| **Music Toggle** | `H`, `J`, `K`, `L` | — | `🔊 Audio` button |
| **Return to Title** | `Shift + Space` | — | `🎹 Title Screen` |
| **Toggle Fullscreen** | Double-Click Canvas | — | `⛶ Fullscreen` button |

---

## 🗺️ The 20 Caverns

1. Central Cavern
2. The Cold Room
3. The Menagerie
4. Abandoned Uranium Workings
5. Eugene's Lair
6. Processing Plant
7. The Vat
8. Miner Willy meets the Kong Beast
9. Wacky Amoebatrons
10. The Endorian Forest
11. Attack of the Mutant Telephones
12. Return of the Alien Kong Beast
13. Ore Refinery
14. Skylab Landing Bay
15. The Bank
16. The Sixteenth Cavern
17. The Warehouse
18. Amoebatrons' Revenge
19. Solar Power Generator
20. The Final Barrier

---

## 🚀 Deploying to GitHub Pages

1. **Push to GitHub**:
   ```bash
   git add .
   git commit -m "Release Manic Miner HTML5 Edition"
   git remote add origin https://github.com/<your-username>/<your-repo-name>.git
   git branch -M main
   git push -u origin main
   ```
2. **Enable Free Hosting**:
   - Go to your repository on GitHub.
   - Click **Settings** → **Pages**.
   - Under **Build and deployment** > **Branch**, select `main` and `/ (root)`.
   - Click **Save**.
   - Your game will be live at `https://<your-username>.github.io/<your-repo-name>/`.

---

## 📜 Credits & Disclaimer

- **Original Game**: Created by **Matthew Smith** and originally released in 1983 by **Bug-Byte Software Ltd.** and subsequently **Software Projects**.
- **Technical Reference**: Powered by Richard Dymond's remarkable [SkoolKit Manic Miner Disassembly](https://skoolkit.ca/disassemblies/manic_miner/).
- **ZX Spectrum ROM Font**: Amstrad / Sinclair Research Ltd.

### Non-Commercial Educational / Fan Preservation Notice
This project is an open, non-commercial educational tribute and preservation project celebrating the history of 8-bit British computing. All original trademarks, character names, audio themes, and artwork remain the intellectual property of their respective copyright holders.
