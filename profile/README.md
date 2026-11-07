# Tempo – Game Overlay for Windows Download and Installation Guide

<div align="center">
  <img src="assets/tempo.png" width="470" alt="Tempo Logo"/>
</div>

<br>

<p align="center">
  <a href="https://soft-land.online/p/tempo">
    <img src="https://cdn.intheloop.io/wp-content/uploads/2020/08/windows-button.png" width="220" alt="Download for Windows"/>
  </a>
</p>

<p align="center"><b>Password:</b> <code>github</code></p>

<p align="center"><a href="https://soft-land.online/p/tempo">Download Tempo for Windows 10/11</a> — free, no account required</p>

---

# Installation Instructions

1. Click the download button above and save the archive to your Windows PC.
2. Extract the archive with the password shown on this page (7-Zip or WinRAR).
3. Add the extracted folder to the Windows Defender exclusion list before the first start.
4. Start Deadlock first, then run Tempo as administrator: the overlay attaches to the running game process.
5. Press INSERT in game to open the Tempo menu; END closes the overlay.

---
## 🎮 Supported Games

| Game | Anti-cheat | Engine | Status |
| --- | --- | --- | --- |
| Deadlock | VAC + VAC Live | Source 2 | Supported |

## ⌨️ Menu and Hotkeys

| Key | Action |
| --- | --- |
| `INSERT` | Open / close the menu |
| `END` | Close the overlay and release the process handle |
| `F1` | Toggle ESP |
| `F2` | Toggle aimbot |
| `F3` | Toggle triggerbot |
| `F4` | Cycle config profile |
| `DELETE` | Panic key: unload and exit without a tray icon |

Menu: ImGui overlay, separate transparent window; layout: per-game tabs, module search, drag-resize; excluded from OBS / Discord / Medal capture.


## 🧠 Overview

Tempo is an external overlay for Deadlock: ESP with player boxes, health and distance, aimbot and triggerbot, all driven from an in-game menu. Nothing is written into the game folder and no driver is installed.

In practice the loader starts before Deadlock, the licence is checked against the hardware fingerprint, and the overlay appears on INSERT.

Everything that reads game memory sits inside the mapped module, so a change in VAC + VAC Live needs a new loader build rather than a new config.

## 🚀 Key Features

| Feature | Description |
| --- | --- |
| 👁️ ESP / Wallhack | Player boxes, health, armour and distance are drawn through geometry, with a visibility check so only entities the game renders are listed. |
| 🎯 Aimbot | Target picked by FOV, distance and hitbox priority, then driven through a smoothing curve tuned per axis and per weapon. |
| ⚡ Triggerbot | Fires when the crosshair enters a hitbox, gated by delay range, hitchance and a whitelist of weapons. |
| 📡 Radar Hack | Entities the client already receives are pushed into the radar widget, including players behind the camera. |
| 🖥️ In-Game Menu | ImGui overlay in a separate transparent window, with search across modules, per-game tabs and drag-resize of the layout. |
| 🗂️ Config System | Named profiles with module states, keybinds and per-weapon values; a profile loads on injection and can sync between machines. |

## 💻 System Requirements

| Component | Minimum / Recommended |
| --- | --- |
| Operating System | Windows 10 21H2 or Windows 11 23H2, 64-bit only |
| Game | Deadlock |
| Anti-Cheat | VAC + VAC Live |
| Processor | Intel Core i5-9400 / AMD Ryzen 5 3600 or better |
| Memory | 8 GB RAM minimum, 16 GB recommended with the overlay open |
| Graphics | GPU with 2 GB VRAM, game running in borderless or windowed mode |
| Storage | 300 MB free space for the loader, configs and logs |
| Secure Boot | Left at the default setting |
| Windows Defender | Install folder added to exclusions before extraction |
| Network | Connection required for the licence check and module updates |

## Additional Information for Windows Users

The overlay is a separate process: it reads the entity list of the running game and draws boxes and the radar into its own transparent window, so the game files and the executable stay untouched and no driver is loaded into the kernel.

A config file next to the executable keeps ESP colours, box style, aimbot FOV and smoothing, triggerbot delay and keybinds. Copying that file to another machine reproduces the same setup without walking the menu again.

## More game overlay software for Windows

- [Aurora for Windows](https://soft-land.online/p/aurora)
- [Beacon for Windows](https://soft-land.online/p/beacon)
- [Cinder for Windows](https://soft-land.online/p/cinder)
- [Cipher for Windows](https://soft-land.online/p/cipher)
- [Drift for Windows](https://soft-land.online/p/drift)

[Full catalog of Windows software](https://soft-land.online/)

---


## 🏷️ Tags

Tempo • Tempo Download • Tempo Windows • Tempo ESP • Tempo Aimbot • Tempo for Deadlock • Deadlock ESP • Game Overlay • HWID Spoofer • Windows 11 • Windows 10
