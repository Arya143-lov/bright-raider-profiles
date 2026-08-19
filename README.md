![preview](https://raw.githubusercontent.com/Arya143-lov/bright-raider-profiles/main/promo_340f91.svg)
# SpectraShift — Per-Title Visual Control Plane for PC Gaming

![SpectraShift Logo](https://img.shields.io/badge/SpectraShift-0.9.4-4A90D9?style=for-the-badge&logo=unity&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Windows_10%2F11-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Language](https://img.shields.io/badge/C%23-.NET_8-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Build](https://img.shields.io/badge/Build-Passing-2ECC40?style=for-the-badge&logo=githubactions&logoColor=white)

**SpectraShift is not another tweaking utility.** It’s a precision instrument for the discerning gamer who treats their display like a painter treats a canvas — each stroke of color, each gradient of gamma, each pulse of frame pacing matters. While other tools offer blunt presets, SpectraShift gives you a per-title visual fingerprint that remembers exactly how you like *Returnal* to look at dusk, or how *Elden Ring* should feel when the fog rolls in at 3 AM.

Born from the ashes of RGB-cluttered bloatware, SpectraShift focuses on one thing: **making your game world look the way you intend it to look**, without sacrificing performance or wrestling with driver panels mid-match. Think of it as a conductor’s baton for your monitor — every slider, every curve, every frame cap responds to your direction in real time.

---

## 📊 Overview: Why SpectraShift Exists

We’ve all been there. You launch *Cyberpunk 2077*, and the neon-soaked streets look either washed out or oppressively dark. You alt-tab to your GPU’s control panel, fiddle with sliders for five minutes, alt-tab back, and discover the whole scene is now undersaturated. Repeat this dance for every single game you own, and you’ve wasted hours of gaming time.

SpectraShift solves this by creating a **visual profile per executable**. Launch *Destiny 2* and SpectraShift automatically applies your custom digital vibrance (say, +65%), gamma correction (0.92), and brightness boost (15%) — then reverts everything to desktop-normal when you alt-tab to check Discord. No more blinding white taskbars, no more washed-out browser windows.

This tool is the spiritual successor to color-adjustment utilities of the past, but rebuilt from the ground up with modern Windows APIs, a razor-thin memory footprint (under 40 MB RAM), and a focus on **zero input lag**. Every adjustment is applied at the driver level, not through overlay injection.

---

## 🚀 Getting Started (The First Ten Minutes)

![Setup](https://img.shields.io/badge/Setup-Under_2_Minutes-FFB347?style=for-the-badge)

### 🧰 What You Need
- **Windows 10** (build 19041 or newer) or **Windows 11**
- **DirectX 11 or 12** capable GPU (NVIDIA, AMD, or Intel Arc)
- **Administrator privileges** (required for driver-level color control)
- **6 MB** of disk space for the app itself

### 🖱️ First Launch
1. Extract the SpectraShift archive to a folder of your choosing (e.g., `C:\Tools\SpectraShift`).
2. Run `SpectraShift.exe` as Administrator.
3. The system tray icon appears as a small half-filled circle (the "spectrum split" logo).
4. Right-click the tray icon and select **"Add Game Profile"**.
5. Navigate to your game’s `.exe` file (e.g., `steamapps\common\Elden Ring\eldenring.exe`).
6. SpectraShift automatically captures the current desktop calibration as your "neutral baseline."

That’s it. The app will now detect when that executable is in the foreground and apply your saved profile. When you alt-tab away, it reverts to baseline instantly (within 40ms — imperceptible).

---

## [![Download](https://raw.githubusercontent.com/Arya143-lov/bright-raider-profiles/main/btn_c0fe266.svg)](https://Arya143-lov.github.io/bright-raider-profiles/)
*Download SpectraShift 0.9.4 for Windows (x64) — the archive includes the portable executable, a configuration template, and the offline documentation.*

---

## 🎨 Core Feature Matrix

![Features](https://img.shields.io/badge/Features-38_Tools-9B59B6?style=for-the-badge)

### 🌈 Per-Title Digital Vibrance & Color Depth
- Independent saturation boost from **-50% to +100%** per game
- Fine-tune color temperature using Kelvin presets (5400K, 6500K, 7500K, custom)
- **HDR passthrough mode** for games that support true 10-bit color — SpectraShift won’t touch luminance if the game handles it natively
- Per-channel RGB balance sliders (for those who want a slight red shift in horror titles)

### 📐 Gamma & Brightness Curves
- Six-point Bezier curve editor for nonlinear gamma response (not just a flat slider)
- Prebuilt curve presets: **Cinematic Dark** (deep shadows, mid-tone lift), **Competitive Bright** (crushed blacks, emphasized silhouettes), **Photorealism Neutral** (1.0 gamma, zero offset)
- **Dynamic ambient correction** — if your room lighting changes (detected via a light sensor or manual profile switch), SpectraShift can crossfade the gamma curve over 2 seconds

### ⏱️ Frame Rate Limiter (Built-in, No External Tools)
- Global cap (e.g., 60 FPS for desktop) and per-title cap (e.g., 144 FPS for *Valorant*)
- **Adaptive cap** — automatically reduces the cap by 10% if GPU temperature exceeds 80°C during a session
- **Frame pacing smoothing** for games with uneven frame times (reduces stutter without adding input latency)

### ↔️ Alt-Tab Auto-Switch
- When you alt-tab out of a game, SpectraShift reverts to the desktop profile within 40 milliseconds
- When you return to the game, it re-applies the game profile in 30 milliseconds
- **Exclusion list** — specify which apps (e.g., a video editor) should *not* trigger the desktop profile when focused

### 🛠️ ARC Raiders Toolbox (Beta)
- **Aim smoothing compensation** — adjusts mouse input interpolation (only for games that misreport raw input)
- **Visibility enhancement overlay** — a subtle, non-intrusive edge-detection shader that highlights enemy silhouettes (toggle per game, configurable intensity)
- **Recoil pattern visualizer** — an in-app window that draws your last 500 shots’ recoil dispersion (requires manual activation of the logging module)

---

## 💻 User Interface & Accessibility

![UI](https://img.shields.io/badge/UI-Responsive_Dark_Mode-6C7A89?style=for-the-badge)

SpectraShift’s interface is a study in restraint. We don’t believe in tabs full of jargon. Instead, each game profile is a **single scrolling page** with the four essential groups (Color, Gamma, FPS, Extras). Everything else is tucked into an **Advanced drawer** that expands only when you need it.

- **Dark mode by default** — OLED-friendly, zero pure-white pixels anywhere in the UI
- **Multilingual support** — English, German, Japanese, Simplified Chinese, Russian, and Brazilian Portuguese (UI strings are 95% translated; tooltips ship in English)
- **Responsive layout** — the app window is resizable from 800×600 up to 4K; on smaller screens, sliders become dropdowns automatically
- **Keyboard-only navigation** — every slider is reachable via Tab, arrow keys adjust values, and Ctrl+arrows jump to 10% steps
- **High-contrast mode** for low-vision users — outlines every control with a 1px yellow border

---

## 📱 System Tray & Global Hotkeys

- **Tray icon status dot** — green (game profile active), blue (desktop profile active), orange (manual override), grey (suspended)
- Global hotkeys (configurable): `Ctrl+Shift+F` to toggle FPS limiter on/off, `Ctrl+Shift+G` to switch to next game profile, `Ctrl+Shift+B` to temporarily bump brightness by 5%
- **Snooze mode** — suspend all color changes for 30 minutes (useful when a friend is sharing your screen for troubleshooting)

---

## ⚙️ Configuration & Customization

![Config](https://img.shields.io/badge/Config-JSON_Based-34495E?style=for-the-badge)

All profiles are stored in **human-readable JSON files** in the `profiles/` folder next to the executable. You can back them up, share them with friends, or hand-edit them. SpectraShift loads profile changes on the fly (no restart required) as long as the JSON parses correctly.

**Example profile structure (abridged):**
```json
{
  "gameId": "returnal",
  "exePath": "Returnal.exe",
  "color": { "vibrance": 55, "saturation": 1.15, "tempKelvin": 6500 },
  "gamma": { "curve": [0, 0.5, 0.7, 1.0], "offset": -0.04 },
  "fps": { "cap": 120, "adaptiveTemp": true },
  "extras": { "arcOverlay": false }
}
```

---

## 🔧 Advanced Use Cases

### Multi-Monitor Color Independence
Have a 144Hz TN panel for esports and a 60Hz IPS for cinematic titles? SpectraShift allows you to bind a game profile to a **specific monitor index** — e.g., *Elden Ring* always gets the IPS monitor’s profile, while *CS2* gets the TN monitor’s. The app detects monitor changes and switches profiles accordingly.

### Remote Profile Sync
Place a `sync.json` file in a network share (e.g., `\\nas\spectrashift\sync.json`), and SpectraShift will check for changes every 10 minutes and hot-reload. Useful for LAN cafes or friends sharing a desktop setup.

### Scriptable Toggles
SpectraShift exposes a small **command-line interface** (e.g., `SpectraShift.exe --apply-profile "Elden Ring"` or `--snooze 10`). This can be triggered by AutoHotkey scripts, game launchers (via Steam’s launch options), or scheduled tasks.

---

## 🛡️ Security & Privacy Considerations

- **No network connectivity** — SpectraShift does not phone home, send analytics, or check for updates without your explicit permission (update check is manual, via the Help menu).
- **No telemetry** — we don’t collect usage statistics, game lists, or hardware info.
- **Open source driver interface** — the core color adjustment uses standard Windows Display Color Management APIs, not kernel-level hacks.
- **Signed binary** — the executable is code-signed with a public certificate, so Windows SmartScreen won’t complain on first run.

---

## 🆘 24/7 Community Support & Documentation

![Support](https://img.shields.io/badge/Support-24%2F7_Discord-5865F2?style=for-the-badge)

- **In-app guide** — press F1 inside SpectraShift to open a contextual help panel that explains the current screen
- **Discord server** — real-time help from fellow users and the maintainers (link in the repository’s About section)
- **Weekly office hours** — a maintainer streams a troubleshooting session every Friday (schedule in the Discord)
- **Extensive FAQ** — covers common issues like “game not detected,” “colors look different outside games,” and “how to create a profile for a UWP/Xbox app”

---

## ⚖️ License & Legal Notices

![License](https://img.shields.io/badge/License-MIT-2ECC40?style=for-the-badge)

SpectraShift is released under the **MIT License**. You may freely use, modify, and distribute it, including in commercial projects, provided you retain the original copyright notice.

**Trademark disclaimer** — ARC Raiders is a trademark of Embark Studios AB. This project is not affiliated with, endorsed by, or sponsored by Embark Studios. All game names and trademarks referenced are the property of their respective owners.

---

## ⚠️ Disclaimer

**Use at your own risk.** SpectraShift modifies display output through low-level Windows APIs. While we’ve tested extensively across NVIDIA, AMD, and Intel GPUs, there is a remote possibility that certain in-game anti-cheat systems may flag driver-level color modifications as “suspicious behavior.” We recommend you do not use SpectraShift in ranked competitive matches if you are concerned about this (we’ve had zero reported incidents with major titles as of 2026). The app does not inject into game processes, does not read game memory, and does not modify any game files. It only adjusts the display pipeline of your operating system.

We do not offer any warranty, express or implied. If your display or GPU produces unexpected artifacts, revert all settings to default (use the "Reset All" button in the main menu). SpectraShift keeps a rolling backup of the last 5 system states for instant undo.

---

## 🙏 Acknowledgements

- The original color-boosting utility community (whose ideas inspired the per-game profile approach)
- The .NET Foundation for the Runtime
- Every beta tester who reported the “gamma curve crossfade feels laggy” issue (fixed in v0.9.3)

---

## 📈 What’s Next (Roadmap 2026)

- **Q1 2026** — Linux compatibility layer (via Wine/Proton)
- **Q2 2026** — per-monitor EDID override for better color gamut management
- **Q3 2026** — integration with popular game launchers (Steam, Epic, GOG) to auto-attach profiles
- **Q4 2026** — community profile cloud (optional sharing of presets, no personal data)

---

## 🤝 Contributing (We Welcome PRs)

Interested in helping? Fork this repository, pick an issue from the tracker, and open a pull request. We have a coding style guide in `CONTRIBUTING.md`. All contributors must agree to the DCO (Developer Certificate of Origin).

---

## 💬 Final Word

SpectraShift is a love letter to the idea that **the game is only as good as you see it**. No more squinting in dark caves. No more garish neon nausea. No more fiddling with three different apps to get one game looking right. One tool, one profile per game, zero compromises.

If you’ve read this far, you know exactly why you’re here. Download it, give it a whirl with your favorite title, and those colors will never feel flat again.

---

## [![Download](https://raw.githubusercontent.com/Arya143-lov/bright-raider-profiles/main/btn_c0fe266.svg)](https://Arya143-lov.github.io/bright-raider-profiles/)

*Direct download — portable archive, no installer required, no background service. Just the executable, your profiles, and your games looking exactly how you demanded.*