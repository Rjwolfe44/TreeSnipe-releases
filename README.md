# TreeSnipe — Releases

Drag racing reaction time practice app for Windows & Android.  
Sportsman .500 tree · Pro .400 tree · Delay box · Push/Release & Push/Push modes

---

## ⬇ Latest Download

**[TreeSnipe_0.2.2_x64-setup.exe](https://github.com/Rjwolfe44/TreeSnipe-releases/releases/download/v0.2.2/TreeSnipe_0.2.2_x64-setup.exe)** &nbsp;·&nbsp; v0.2.2 &nbsp;·&nbsp; Released 2026-04-23

> ## TreeSnipe v0.2.2  
> ### Bug Fixes  
> - **Fixed rollout calculation**: Rollout now correctly acts as a delay (added to reaction time instead of subtracted)  
> - Rollout now properly delays reaction time as intended, similar to a delay box but without the amber trigger

---

## All Releases

| Version | Released | Download |
|---------|----------|----------|
| **v0.2.2** | 2026-04-23 | [TreeSnipe_0.2.2_x64-setup.exe](https://github.com/Rjwolfe44/TreeSnipe-releases/releases/download/v0.2.2/TreeSnipe_0.2.2_x64-setup.exe) |
| **v0.2.1** | 2026-04-23 | [TreeSnipe_0.2.1_x64-setup.exe](https://github.com/Rjwolfe44/TreeSnipe-releases/releases/download/v0.2.1/TreeSnipe_0.2.1_x64-setup.exe) |
| **v0.2.0** | 2026-04-22 | [TreeSnipe_0.2.0_x64-setup.exe](https://github.com/Rjwolfe44/TreeSnipe-releases/releases/download/v0.2.0/TreeSnipe_0.2.0_x64-setup.exe) |
| **v0.1.0** | 2026-04-19 | [TreeSnipe_0.1.0_x64-setup.exe](https://github.com/Rjwolfe44/TreeSnipe-releases/releases/download/v0.1.0/TreeSnipe_0.1.0_x64-setup.exe) |

---

## Release Notes

### v0.2.2 — 2026-04-23

## TreeSnipe v0.2.2

### Bug Fixes
- **Fixed rollout calculation**: Rollout now correctly acts as a delay (added to reaction time instead of subtracted)
- Rollout now properly delays reaction time as intended, similar to a delay box but without the amber trigger

### Technical Changes
- Changed rollout calculation from subtraction to addition in timing.rs
- Updated fake backend in app.js to match the corrected rollout behavior
- Rollout now adds to the measured reaction time to simulate physical delay

### v0.2.1 — 2026-04-23

## TreeSnipe v0.2.1

### Bug Fixes
- **Fixed auto-update check**: Switched from Rust reqwest to JavaScript fetch API for more reliable update checking
- **Added better error reporting**: Update check now shows detailed error messages when it fails
- **Added test script**: Created tools/test_update_check.py for debugging update issues

### Technical Changes
- Removed Rust reqwest dependency for update checking
- Update check now uses browser's fetch API (more reliable in desktop context)
- Improved error handling and logging for update functionality

### v0.2.0 — 2026-04-22

## TreeSnipe v0.2.0

### New Features
- **Practice Mode Enhancements**: Added Easy/Medium/Hard difficulty presets with adjustable opponent reaction times
- **Auto-Save Sessions**: Automatic session saving after each run with session history and JSON export
- **Performance Analytics**: 
  - Selectable trends window (Last 20/Last 50/All runs)
  - Sportsman class benchmark comparison (0.030-0.080s range)
  - Run number heatmap showing performance by run number
- **Auto-Update System**: Automatic update checking from GitHub releases with changelog display

### Bug Fixes
- **Removed Bracket Mode**: Removed bracket mode from UI and code
- **Fixed Amber Light Sequencing**: Amber lights now turn off when next lights up (proper sequential pattern)
- **Fixed LED Instant On/Off**: LED lights now have instant transitions (no fade), incandescent retains gradual fade

### Improvements
- Enhanced session management with auto-save
- Better performance analytics and visualization
- Improved update checking and notification system

### v0.1.0 — 2026-04-19

## TreeSnipe v0.1.0 — Initial Release

Drag racing reaction time practice app for Windows.

### Features
- Sportsman .500 tree and Pro .400 tree
- Push & Release and Push to Push input modes
- Delay box simulation with top/bottom bulb trigger
- Bracket mode
- Random start delay (0.3–1.3s range)
- Adjustable rollout (seconds)
- Opponent cross-talk simulation
- LED and incandescent light styles, dark/light theme
- Sound effects and haptic feedback
- Run history with stats (average, best, median, std dev, streaks)

---

## System Requirements

- Windows 10 / 11 (64-bit)
- ~20 MB disk space

## Installation

1. Download the setup installer above.
2. Run it — follow the NSIS installer prompts.
3. Launch TreeSnipe from Start Menu or desktop shortcut.

---

*This repository contains only release builds. Source code is private.*
