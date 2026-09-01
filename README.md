# RotatoCAM — Free 4-Axis Rotary CAM & G-code Generator for DIY CNC

**Turn an STL or STEP into simultaneous 4-axis rotary G-code — without an expensive CAM subscription.**
A from-scratch CAM program for hobby machinists with a rotary (4th) axis, running **grblHAL · GRBL · Genmitsu · AtomStack · HolzProfi HC-204A · LinuxCNC · Mach3/Mach4 · Centroid · MASSO** — plus drop-in custom posts for anything else. Free Community Edition for Windows.

![Version](https://img.shields.io/badge/version-0.69.2.223.17-ffb000)
![Price](https://img.shields.io/badge/community%20edition-free-46d17a)
![Platform](https://img.shields.io/badge/Windows-10%20%2F%2011-555)

Lay a model in the chuck and get **continuous simultaneous X+C+Z** roughing and finishing toolpaths, **wrapped rotary engraving**, and **flat 2D engraving** — with a 3D backplot and a material-removal simulation so you can verify the program before you ever cut.

> ⚠️ **EXPERIMENTAL — read this before you cut.** RotatoCAM only *writes* a G-code file; it does **not** run your machine, and its output is only a **suggestion you must verify**. CNC mills, lasers and plasma cutters are dangerous. **You alone are responsible** for inspecting every program, air-cutting first, and operating safely. Provided **AS-IS, with no warranty**.

> 🆕 **New in 0.69.2.223.17: a 3+1 safety fix, and Makera Carvera support.**  Bug reports welcome at **therealrevjmoney@gmail.com**.

## Download

- **Free Community Edition** — grab the portable Windows zip from [**Releases**](../../releases) (unzip and run, no install, no admin rights), or from **https://rotatocam.com/**
- **RotatoCAM Pro** — all strategies + conversational (no-CAD) programming + a built-in 4-axis G-code viewer (RotatoVIEW): **https://rotatocam.com/**

**New to rotary CAM?** A quick How-To (load → pick a strategy → Generate → Simulate → Export) lives at **https://rotatocam.com/#how-to** and in the app under **Help → Getting started**. Bundled example projects (fluted columns, a camshaft, engraving) open from **Help → Open example projects…**.

## What it does

- **Simultaneous 4-axis rotary surfacing** — spiral finishing + radial roughing straight from an STL or STEP solid, around the C axis
- **Wrapped rotary engraving** — system-font text or DXF/SVG wrapped onto a round bar with a real V-bit profile
- **Flat 2D engraving** — multi-line text and drawings on a plane
- **STL & STEP/STP import** — load meshes or CAD solids directly (solids are tessellated and scaled to mm)
- **Verify before iron** — 3D backplot, a feed/units check, and a deviation-colored material-removal simulator with a machining-time estimate
- **Posts:** grblHAL, GRBL (3018 / 3040), **Genmitsu / SainSmart** (4040-PRO, 3030 PROVer MAX — grbl 1.1f with a real 4th axis), **AtomStack C4 Pro** (native A axis in degrees, experimental), **HolzProfi CNC6090 / HC-204A** (4-axis linkage, rotary about machine Y, experimental), LinuxCNC, Mach3 / Mach4, Centroid (Acorn / Oak), MASSO G2/G3 (experimental) — plus **drop-in custom posts** (add your own controller from a folder, no rebuild) · **mm / inch** output
- **Portable** — Python and every dependency bundled; nothing to install

## Editions

| | Community Edition — Free | Pro — $49 |
|---|---|---|
| **Price** | Free forever | Pay once per major version (no subscription) |
| **Strategies** | 4-axis finish (spiral) · 4-axis rough (radial) · flat 2D engrave · wrap engrave | **Everything in CE**, plus raster + axial/flow finishing, helical roughing, 3+1 indexed surfacing, pencil cleanup, V-carve, the full conversational suite, adaptive roughing, and laser/plasma 2D cutting |
| **Safety + setup workflow, backplot, simulation** | ✓ | ✓ |

The free edition is genuinely useful on its own — take a rotary part from model to verified G-code. Pro unlocks the deep toolbox: **https://rotatocam.com/**

## Requirements

64-bit **Windows 10/11** · 4-core CPU · 8 GB RAM · a GPU with **OpenGL 3.2+** (integrated is fine) · ~2 GB disk.

## License

RotatoCAM Community Edition is **free to download and use** (closed-source freeware). The full terms are shown in the app under **Help → About** and ship with the download.

---

Website · downloads · Pro: **https://rotatocam.com/** · Contact: **therealrevjmoney@gmail.com**
Built in Myrtle Beach by Rev. J. Money.
