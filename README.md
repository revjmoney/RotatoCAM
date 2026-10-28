<p align="center">
  <img src="assets/rotatocam-logo.png" alt="RotatoCAM logo" width="128" height="128">
</p>

# RotatoCAM

**Spin the stock. Read the signal.**

Free (and pro version) 4-axis rotary CAM and G-code generator for DIY CNC. Turn an STL or STEP into
simultaneous 4-axis rotary toolpaths, wrapped engraving, and a verified material-removal
simulation on Windows, without a CAM subscription.

![Price](https://img.shields.io/badge/community%20edition-free-46d17a)
![Platform](https://img.shields.io/badge/Windows-10%20%2F%2011-555)

> ⚠️ **EXPERIMENTAL.** RotatoCAM only writes a G-code file; it does not run your machine,
> and its output is only a suggestion you must verify. CNC machines are dangerous. You alone
> are responsible for inspecting every program, air-cutting first, and operating safely.
> Provided AS-IS, with no warranty.

<p align="center">
  <a href="https://youtu.be/nLq4axAjO8o"><img src="https://img.youtube.com/vi/nLq4axAjO8o/maxresdefault.jpg" alt="Watch: Rotary CNC CAM Made Simple, the RotatoCAM walkthrough" width="560"></a><br>
  <sub>▶ <b>New here?</b> Watch <a href="https://youtu.be/nLq4axAjO8o">Rotary CNC CAM Made Simple: The RotatoCAM Walkthrough</a></sub>
</p>

## Download

Grab the free Community Edition at **[rotatocam.com](https://rotatocam.com/#download)**.
Unzip and run: no install, no license, no expiry.

Everything else lives there too: what it does, the how-to, the gallery, the safe-testing
guide, supported controllers, and RotatoCAM Pro.

<p align="center">
  <a href="https://youtu.be/-k3qV4LQ3jc"><img src="https://img.youtube.com/vi/-k3qV4LQ3jc/hqdefault.jpg" alt="Watch: RotatoCAM STL to 4-Axis Rotary G-code in Minutes" width="480"></a><br>
  <sub>▶ Quick start: <a href="https://youtu.be/-k3qV4LQ3jc">STL to 4-Axis Rotary G-code in Minutes</a></sub>
</p>

## Screenshots

### Pikachu rotary simulation

Material-removal simulation showing the Pikachu model between the remaining stock ends.

![Pikachu rotary material-removal simulation](assets/screenshots/rotatocam-pikachu-sim.png)

### Pawn toolpaths

Rotary toolpath preview with the pawn model and chuck fixture in view.

![Pawn rotary toolpaths and chuck fixture in RotatoCAM](assets/screenshots/rotatocam-pawn-toolpath.png)

<p>
  <a href="https://www.youtube.com/shorts/U1BHMhwmi10"><img src="https://i.ytimg.com/vi/U1BHMhwmi10/oar2.jpg" alt="Watch: toolpath generation from an STL model" width="140"></a><br>
  <sub>▶ Watch toolpaths get generated from an STL model (<a href="https://www.youtube.com/shorts/U1BHMhwmi10">Twitch clip</a>)</sub>
</p>

### Engraving simulation

Engraving playback with the cutter, toolpath, and G-code readout visible.

![Engraving simulation with toolpath and G-code playback](assets/screenshots/rotatocam-engrave-iso.png)

## See it in action

RotatoCAM on a DIY 4th axis. Click any thumbnail to watch on YouTube.

<p align="center">
  <a href="https://youtu.be/NhmXwB_GKhM"><img src="https://img.youtube.com/vi/NhmXwB_GKhM/maxresdefault.jpg" alt="Watch: 4th axis tiki carved in one pass on the rotary" width="560"></a><br>
  <sub>▶ <a href="https://youtu.be/NhmXwB_GKhM">Tiki carved in one pass on the rotary</a></sub>
</p>

### Rough → spiral finish

Continuous rotary spiral finishing: the A axis keeps turning while the cutter walks along the part.

<p align="center">
  <a href="https://youtu.be/-dh9E5Rkhbc"><img src="https://img.youtube.com/vi/-dh9E5Rkhbc/maxresdefault.jpg" alt="Watch: Continuous 4-Axis Rotary Spiral Finishing" width="480"></a><br>
  <sub>▶ <a href="https://youtu.be/-dh9E5Rkhbc">Continuous 4-Axis Rotary Spiral Finishing (grblHAL)</a></sub>
</p>

<table>
<tr>
<td align="center" width="50%">
<a href="https://youtu.be/-pbEa4EvQ14"><img src="https://img.youtube.com/vi/-pbEa4EvQ14/maxresdefault.jpg" alt="Watch: milling a Walter White bust on the 4th axis" width="360"></a><br>
<sub>Walter White bust, rough → spiral finish</sub>
</td>
<td align="center" width="50%">
<a href="https://youtu.be/4CAcZ1Mt4Xs"><img src="https://img.youtube.com/vi/4CAcZ1Mt4Xs/maxresdefault.jpg" alt="Watch: milling an M4 flash hider on the 4th axis" width="360"></a><br>
<sub>M4 flash hider, rough → spiral finish</sub>
</td>
</tr>
<tr>
<td align="center" width="50%">
<a href="https://youtu.be/lFJX--Dj7-U"><img src="https://img.youtube.com/vi/lFJX--Dj7-U/maxresdefault.jpg" alt="Watch: wrapping a V8 camshaft on the 4th axis" width="360"></a><br>
<sub>V8 camshaft, rough → spiral finish</sub>
</td>
<td align="center" width="50%">
<a href="https://youtu.be/K1r1PqGf7oc"><img src="https://img.youtube.com/vi/K1r1PqGf7oc/maxresdefault.jpg" alt="Watch: BREAKING NEWS, RotatoCAM is pushing rotary 4th axis machining to its limits" width="360"></a><br>
<sub>🚨 BREAKING NEWS: pushing the rotary to its limits</sub>
</td>
</tr>
</table>

### How it started

The first rotary experiments on a DIY 4-axis mini mill, before RotatoCAM had a name.

<table>
<tr>
<td align="center" width="50%">
<a href="https://youtu.be/3nyX98AkQQw"><img src="https://img.youtube.com/vi/3nyX98AkQQw/maxresdefault.jpg" alt="Watch: first 4th axis toolpaths on a DIY 4 axis mini CNC mill" width="360"></a><br>
<sub>First 4th axis toolpaths on the DIY mini mill</sub>
</td>
<td align="center" width="50%">
<a href="https://youtu.be/MWDd28InmpQ"><img src="https://img.youtube.com/vi/MWDd28InmpQ/maxresdefault.jpg" alt="Watch: 4th axis rotary milling a spine keychain" width="360"></a><br>
<sub>4th axis rotary: milling a spine keychain</sub>
</td>
</tr>
</table>

## Why no CAM subscription?

Because some CAM "deals" feel a little like this. A totally fictional undercover documentary:

<p align="center">
  <a href="https://youtu.be/kdwuH8-2fAQ"><img src="https://img.youtube.com/vi/kdwuH8-2fAQ/maxresdefault.jpg" alt="Watch: UNDERCOVER: The CAM Cartels" width="560"></a><br>
  <sub>▶ <a href="https://youtu.be/kdwuH8-2fAQ">🕵️ UNDERCOVER: The CAM Cartels | Inside the Shady World of Expensive CAM Software</a></sub>
</p>

<p align="center">
  <a href="https://www.youtube.com/shorts/PCUCCy3nEVg"><img src="https://i.ytimg.com/vi/PCUCCy3nEVg/oar2.jpg" alt="Short: Undercover with the CAM Cartels" width="160"></a>
  <a href="https://www.youtube.com/shorts/Gbxlb_edQQo"><img src="https://i.ytimg.com/vi/Gbxlb_edQQo/oar2.jpg" alt="Short: The CAM Smugglers at the Marina" width="160"></a>
  <a href="https://www.youtube.com/shorts/31AFaaiVW74"><img src="https://i.ytimg.com/vi/31AFaaiVW74/oar2.jpg" alt="Short: The Laundromat CAM Informant" width="160"></a>
  <a href="https://www.youtube.com/shorts/66LjMKaU65w"><img src="https://i.ytimg.com/vi/66LjMKaU65w/oar2.jpg" alt="Short: Monthly CAM Payments at the Motel" width="160"></a>
  <br>
  <sub>Shorts: Undercover with the CAM Cartels · The CAM Smugglers at the Marina · The Laundromat CAM Informant · Monthly CAM Payments at the Motel</sub>
</p>

<sub>Parody. All characters, companies, and product names in it are made up.</sub>

## More from the shop

<details>
<summary><b>Unlocking locked cutting machines (KillCric open firmware)</b></summary>

<br>

<table>
<tr>
<td align="center" width="50%">
<a href="https://youtu.be/GoS-c16rHFs"><img src="https://img.youtube.com/vi/GoS-c16rHFs/maxresdefault.jpg" alt="Watch: I Cracked Open a Locked CNC Machine" width="360"></a><br>
<sub>I Cracked Open a Locked CNC Machine: It Runs GPLv3 Software They Won't Release</sub>
</td>
<td align="center" width="50%">
<a href="https://youtu.be/PNrlSQWWdnY"><img src="https://img.youtube.com/vi/PNrlSQWWdnY/maxresdefault.jpg" alt="Watch: They Locked This Vinyl Cutter Behind a Cloud" width="360"></a><br>
<sub>They Locked This Vinyl Cutter Behind a Cloud, So I Tore It Open</sub>
</td>
</tr>
<tr>
<td align="center" width="50%">
<a href="https://youtu.be/sMOpH-vP6b4"><img src="https://img.youtube.com/vi/sMOpH-vP6b4/maxresdefault.jpg" alt="Watch: Turning a Cricut Expression Into a Real CNC Machine" width="360"></a><br>
<sub>Turning a Cricut Expression Into a Real CNC Machine</sub>
</td>
<td align="center" width="50%">
<a href="https://youtu.be/umrlLP49aIY"><img src="https://img.youtube.com/vi/umrlLP49aIY/maxresdefault.jpg" alt="Watch: This Cricut Has No Account, No Cartridges, No Subscription" width="360"></a><br>
<sub>No Account, No Cartridges, No Subscription: KillCric Open Firmware</sub>
</td>
</tr>
</table>

Short: [This "locked" machine is secretly open source 🔓](https://www.youtube.com/shorts/wbDPPe3ATIM)

</details>

<details>
<summary><b>The 3-axis days: 3018 mini mill archive</b></summary>

<br>

Before the rotary, there was a little 3018. Mostly live streams.

- [Milling The SOA Reaper on a 3018 CNC](https://youtu.be/4LxdE0r-6d0)
- [3018 Toolpath CNC MILLING W Fusion 360 Toolpaths](https://youtu.be/qH6AEFYYP7U)
- [3018 cnc mill and Fusion 360 make a bee thing!](https://youtu.be/jNXKMgR0X5c)
- [3018 Toolpath Simulation in Fusion 360!](https://youtu.be/qRn7Loa1hfc)
- [CNC MILLING a baby sword plaque](https://youtu.be/IBQ5mcxzXYY)
- [CNC MILLING a baby monkey from cherry wood using fusion 360 toolpaths](https://youtu.be/XZt1UUsSoCg)
- [CNC MILLING a cherry wood pipe on the 3018 mini mill](https://youtu.be/x9SGPmoJfKI)
- [CNC MILLING a cherry wood pipe on the 3018](https://youtu.be/RGkWLmDuHZQ)
- [CNC MILLING a pipe from holly wood on the 3018 (stream2)](https://youtu.be/Zu0BtocLtiw)
- [CNC MILLING a pipe from holly wood on the 3018 cnc mill](https://youtu.be/piT8JKVfda8)
- [3018 cnc v carving a sign](https://youtu.be/UFdPQTdqSi0)
- [3018 MILLING SMALL KEYCHAIN TEST](https://youtu.be/-HGXWtMy7EQ)
- [3018 cnc mill live stream, milling random stuff!](https://youtu.be/dqIJ4sGhk_U)
- [3018 cnc milling random stuff](https://youtu.be/DOhWHO6mrDs)
- [3018 cnc milling a monkey from holly wood with fusion 360 toolpaths!](https://youtu.be/bYTPo_8siQI)
- [3018 cnc milling a monkey from holly wood with fusion 360 toolpaths! (another stream)](https://youtu.be/TOtuPRNhYk8)
- [3018 cnc mini milling a monkey mask in wood](https://youtu.be/POthWUIpVA8)
- [live 3018 cnc mill, some Holly Wood, fusion 360!](https://youtu.be/IY1iYGp5Wf0)
- [3018 cnc mill, 3d carving a skull in acrylic rod](https://youtu.be/eBKaGJe5-cI)
- [3018 milling a 5" ashtray from wood cutting board](https://youtu.be/KA2PLKFao38)
- [engraving stuff on the 3018 mini mill/router](https://youtu.be/dCa0X1J-lLY)

</details>

More on the channel: **[@REVJMONEY on YouTube](https://www.youtube.com/@REVJMONEY)**

---

Built in Myrtle Beach by Rev. J. Money · **https://rotatocam.com/** · therealrevjmoney@gmail.com
