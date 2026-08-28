# RotatoCAM — Free 4-Axis Rotary CAM & G-code Generator for DIY CNC

**Turn an STL or STEP into simultaneous 4-axis rotary G-code — without an expensive CAM subscription.**
A from-scratch CAM program for hobby machinists with a rotary (4th) axis, running **grblHAL · GRBL · Genmitsu · AtomStack · HolzProfi HC-204A · LinuxCNC · Mach3/Mach4 · Centroid · MASSO** — plus drop-in custom posts for anything else. Free Community Edition for Windows.

![Version](https://img.shields.io/badge/version-0.69.2.223.16-ffb000)
![Price](https://img.shields.io/badge/community%20edition-free-46d17a)
![Platform](https://img.shields.io/badge/Windows-10%20%2F%2011-555)

Lay a model in the chuck and get **continuous simultaneous X+C+Z** roughing and finishing toolpaths, **wrapped rotary engraving**, and **flat 2D engraving** — with a 3D backplot and a material-removal simulation so you can verify the program before you ever cut.

> ⚠️ **EXPERIMENTAL — read this before you cut.** RotatoCAM only *writes* a G-code file; it does **not** run your machine, and its output is only a **suggestion you must verify**. CNC mills, lasers and plasma cutters are dangerous. **You alone are responsible** for inspecting every program, air-cutting first, and operating safely. Provided **AS-IS, with no warranty**.

> 🆕 **New in 0.69.2.223.16: Makera Carvera support.** A native post for the whole Carvera
> family (C1 / Air / Z1) plus built-in machine presets: pick your model in Machine setup and the
> travels, swing radius, chuck figures, feed cap and the right controller are filled in for you.
> The post follows the Carvera Community Profiles conventions (Smoothieware dialect, parenthesised
> comments, G94 linear + G93 inverse-time rotary, G28 + M30 ending), pins the rotary letter to A
> (the firmware errors on B or C, so RotatoCAM never emits them), and saves programs as **.cnc**.
> Contributed as a community handoff by a Carvera owner - thank you, ExaltedRaddix. ⚠ Not yet
> verified by cutting on a Carvera: air-cut your first program. Also in this release: the export
> extension now follows the controller (.ngc for LinuxCNC), and 3+1 indexed work survives model
> slices that the mesh library refuses to repair (organic / AI-exported meshes) instead of failing
> the whole Generate.
> *(From 0.69.2.223.15: An accurate rotary drop cutter for every wrapped strategy.
> Each rotation angle now casts a dense lateral band of rays reduced through the tool's true
> profile: on the ball-on-sphere closed form the error drops from ~0.15 mm into the hundredths,
> and a tapered cutter rests on its actual cone instead of being planned as its shank. Cut radii
> move slightly outward, never inward. **Roughing leaves its allowance perpendicular to the
> part**, so 0.5 mm on a shoulder is 0.5 mm, not 0.36. **The sim playback stopped lying twice
> over:** the on-screen cutter now rides the cut surface instead of orbiting through the billet
> as the chuck turns, and tracks the real machine Y across a clocked 3+1 face. **One Path switch
> now governs every toolpath line in the app** — lit means lines on screen, off means a clean
> cutter-and-material view, instantly both ways. **The log panel can be hidden** from Settings.
> *(From 0.69.2.223.14: Safe Z became a clearance above the STOCK SURFACE — it used to be measured
> from the rotary axis, so on a part of any size the number was nonsense: set 10 mm on a part with a
> 14 mm radius and your retract was 4 mm *inside* the material. It is now a clearance **above the
> stock surface** — type 10 and the tool pulls up 10 mm clear of the work, and the exported file says
> `Z10` too. The change can only ever raise a retract, never lower one. **Header comments a
> controller can actually parse:** the lines at the top of the program ran past grbl's 80-character
> line buffer and, on posts whose name contained brackets, put brackets inside brackets, which ends
> a comment early so the rest of the line is read as G-code. A dry run reported
> `error:11, error:2, error:11, error:2` and never got past the header. Fixed for every post at once.
> **A new install now opens in the plain light theme**, looking like an ordinary desktop application;
> the dark, CRT green and amber themes are all still under Settings. **Mill / Laser / Plasma moved to
> Settings ▸ Machine mode**, behind a confirmation, because it sat next to Controller and one stray
> click silently hid every rotary strategy including 3+1. **Feeds for tapered and V cutters were far
> too fast** — chip load was sized off the shank rather than the tip that is actually cutting. Plus
> a **HolzProfi CNC6090 / HC-204A post**, a rotary-letter picker that greys out when the controller
> only speaks one letter, and an **opt-in out-of-travel check** that stays silent until you tell it
> where your work zero is. From 0.69.2.223.13: **a rotary mounted along Y now works** — the new
> Rotary runs along setting rotates the emitted program a quarter turn so the part's length comes out
> on Y, a true rotation rather than an axis swap, so nothing is mirrored. And **the app tells the
> update feed which version it is**, the version string and nothing else. From 0.69.2.223.12: **the simulator no longer eats the part when the cutter
> works near the rotary axis** — a 3+1 job on a part with openings on the centreline could come out
> of the sim as a thin pin down the middle while the G-code was correct the whole time. **Tapered
> cutters are planned as the shape they are** — choose *taper* as the tool type, give it an included
> angle and a tip diameter, or a corner radius for a tapered ball nose, and pass spacing solves your
> scallop against the real cutter profile. **The AtomStack C4 Pro is supported**, its rotary treated
> as a real fourth axis in plain degrees rather than a substituted Y, with absolute angles past a
> full turn preserved. **There is a French option** for the safety gate and the getting-started
> guide, under Settings ▸ Language. **The bundled example projects open** — nine models and
> eighteen ready-to-run job sheets were inside every download all along, but the portable build
> looked for them one folder too high. And **a square billet is checked as a square billet**, on Y
> and Z one axis at a time.)* Bug reports welcome at **therealrevjmoney@gmail.com**.

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
