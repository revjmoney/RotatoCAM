# RotatoCAM — Affordable 4-Axis Rotary CAM for DIY CNC

**Take a 3D model straight to G-code for a rotary (4th-axis) setup — without paying four figures for a CAM seat.**

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-lightgrey)
[![Download](https://img.shields.io/badge/download-Releases-orange)](../../releases/latest)

RotatoCAM is a from-scratch **CAM / G-code generator** for DIY CNC machines with a table-mounted **rotary (4th / C) axis** — mini knee mills, 3018/3040 routers, anything running **grblHAL, GRBL, or LinuxCNC**. It does real **simultaneous 4-axis rotary roughing and finishing**, wrapped rotary engraving, and flat 2D engraving, with a built-in **backplot and material-removal simulation** so you verify before you cut.

This is the **Community Edition — free software (GPLv3)**. A **Pro** edition ($49, no subscription, pay once per major version) adds the heavier strategies. **[Download + details → jmscnc.com/rotatocam](https://jmscnc.com/rotatocam)**

📺 **Demo:** [Continuous 4-axis rotary spiral finishing](https://youtu.be/-dh9E5Rkhbc)

## Download & run
Grab the latest **portable Windows build** from the **[Releases page](../../releases/latest)** (or from [jmscnc.com/rotatocam](https://jmscnc.com/rotatocam)). No install, no Python needed:

1. Download the `RotatoCAM-…-Windows-portable.zip`
2. Unzip it anywhere
3. Run `RotatoCAM.exe`

> Not code-signed, so Windows SmartScreen may say *"Windows protected your PC"* on first run — click **More info → Run anyway**.

## Why this exists
$15k for simultaneous 4-axis in Fusion is a joke. DeskProto is clunky, Vectric is pricey and wood-first. I had a DIY 4th axis and no sane CAM for it — so I wrote one. It's not trying to be Mastercam; it's trying to get your part cut.

## Features (Community Edition)
- **Simultaneous 4-axis rotary** — roughing (radial) + finishing (spiral)
- **Wrapped rotary engraving** — text/art around a cylinder
- **Flat 2D engraving**
- **Import:** STL · STEP/IGES · OBJ · 3MF · DXF · SVG
- **Backplot + material-removal simulation**
- **Posts:** grblHAL · GRBL · LinuxCNC
- Runs forever — no license, no nag, no subscription

## Community vs Pro
| | Community (free) | Pro ($49) |
|---|---|---|
| Rotary finishing | Spiral | + raster, axial/flow |
| Rotary roughing | Radial | + helical |
| Wrapped + flat engraving | ✅ | ✅ |
| STEP / IGES import | ✅ | mesh only |
| 3+1 indexed surfacing, pencil cleanup, V-carve | — | ✅ |
| Conversational (no-CAD) suite, adaptive roughing | — | ✅ |
| Laser / plasma 2D cutting | — | ✅ |
| Backplot + simulation · grblHAL/GRBL/LinuxCNC | ✅ | ✅ |

## ⚠️ Safety
RotatoCAM only **writes** G-code — **it does not run your machine.** CNC mills, lasers, and plasma are dangerous. Always review the backplot, run the simulation, and **air-cut** every program before you cut. Provided **AS-IS, no warranty** — you are the operator and you are responsible.

## License & source
RotatoCAM Community Edition is **free software under the GNU GPL v3**. You may use, study, share, and modify it under those terms.

**Corresponding source:** the source for each release is available on request — email **therealrevjmoney@gmail.com** and I'll send you the source for that build. (The Pro edition is a separate, proprietary product.)

---
*Built by [Rev. J. Money](https://jmscnc.com) / JMS CNC — because affordable 4-axis rotary CAM should exist.*
