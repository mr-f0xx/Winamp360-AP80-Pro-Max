# Winamp 360 — AP80 Pro Max

A **Winamp Classic-inspired Rockbox theme** for the **Hidizs AP80 Pro Max**, drawn natively for its 360 × 640 portrait display. Dark navy brushed-metal Winamp surfaces, authentic logo, classic electric-blue selection, dynamic bouncing spectrum visualizer, tactile transport keys, and signature green & yellow accents.

[**Download Latest Release**](https://github.com/mr-f0xx/Winamp360-AP80-Pro-Max/releases/latest)

<p align="center">
  <img src="previews/now-playing-360x640.png?v=3" width="360" height="640" alt="Winamp 360 Now Playing View (360x640)">
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="previews/main-menu-360x640.png?v=3" width="360" height="640" alt="Winamp 360 Main Menu View (360x640)">
</p>

<p align="center">
  <em>Now Playing view (left) and Main Menu view (right) rendered at native 360 &times; 640 resolution.</em>
</p>

## What it is

Winamp 360 is an original Rockbox theme crafted specifically for the **Hidizs AP80 Pro Max**. It includes:
- **Now Playing Screen (WPS)** with cover art, animated stereo analyzer, seek/volume rails, tactile transport controls, and direct navigation buttons.
- **Main Menu Screen (SBS)** with synchronized Winamp masthead, classic electric-blue selection bar with Winamp yellow text, and live Now Playing footer.
- **Charge Dashboard** automatically triggered during USB charging with battery percentage, pack voltage, and status.
- **Theme Configuration (`Winamp360.cfg`)** and bundled fonts.

## Features

### Now Playing View
- **Status Masthead:** Clock on the left (`11:29`), authentic 3D Winamp logo centered in the middle, and enlarged battery percentage + segmented battery icon on the right, all aligned along a unified vertical axis (`y=29`).
- **LCD Status Window:** Digital track timer, playback state, scrolling title, artist, album, and audio format line (`FLAC / kbps / kHz`).
- **Cover Art:** 216 &times; 216 album art in a 220 &times; 220 beveled frame, paired with a custom dark vinyl grooved fallback with golden Winamp bolt when no artwork is available.
- **Dynamic EQ Visualizer:** 10-frame animated 18-band spectrum analyzer with floating peak caps, authentic LED color ladder (green &rarr; orange &rarr; red), and seamless dark chassis integration (no black box cutouts).
- **Classic Winamp Sliders:**
  - **Seek Bar:** Authentic uncolored dark grooved track matching the classic Winamp default theme, featuring an enlarged champagne-gold tactile thumb button (`30 × 16 px`) with a recessed horizontal slot.
  - **Volume Bar:** Vibrant Winamp orange rail (`#D87818`) with beveled silver thumb button featuring 3 vertical tactile slits (`|||`).
- **Tactile 3D Transport Keys:** 5 brushed-metal keys (52 × 42 px) with clean straight bevels and drop wells: Shuffle, Previous, Play/Pause, Next, and Repeat.
- **Direct Navigation Bar:** Quick tactile buttons for `BROWSE`, `QUEUE`, and `MENU`.

### Main Menu View (SBS)
- **Unified Masthead:** Matches the Now Playing masthead with identical clock, logo, and battery placement for seamless visual transitions.
- **Centered Menu Title:** "MAIN MENU" header centered directly under the Winamp logo.
- **Classic Winamp Selection:** Electric blue highlight bar (`#0000C6`) with authentic Winamp yellow active text (`#E7D42F`), while unselected items display in terminal green (`#00FF00`).
- **Live Footer:** Compact Now Playing footer with track title, artist, playback indicator, and remaining track time rendered in green with the digital LCD font (`20-digital7mono.fnt`).

### Touch Controls

Every control on the Now Playing screen features generous touch targets for easy thumb navigation:

| Control | Type | Action |
| ------- | ---- | ------ |
| **Shuffle** | 52 &times; 42 key | `shuffle` toggle |
| **Previous** | 52 &times; 42 key | `wps_prev` |
| **Play / Pause** | 52 &times; 42 key | `play` toggle |
| **Next** | 52 &times; 42 key | `wps_next` |
| **Repeat** | 52 &times; 42 key | `repmode` toggle |
| **Seek Bar** | Full 320 px rail | `progressbar` — drag to scrub |
| **Volume Bar** | Full 238 px rail | `volume` — drag to adjust level |
| **BROWSE / QUEUE / MENU** | 100 &times; 25 each | `browse` / `playlist` / `menu` |

## Installation

1. Download **`Winamp360-AP80-Pro-Max.zip`** from the [Latest Release](https://github.com/mr-f0xx/Winamp360-AP80-Pro-Max/releases/latest).
2. Connect your Hidizs AP80 Pro Max via USB (in Mass Storage mode) or insert its microSD card into your computer.
3. Extract the zip file directly to the root of the microSD card. Ensure the `.rockbox` directory structure merges with your existing installation:
   - `/.rockbox/themes/Winamp360.cfg`
   - `/.rockbox/wps/Winamp360.wps`
   - `/.rockbox/wps/Winamp360.sbs`
   - `/.rockbox/wps/Winamp360/` (bitmaps)
   - `/.rockbox/fonts/` (bundled fonts)
4. Safely eject the player. On the device, go to **Settings → Theme Settings → Browse Theme Files** and select `Winamp360.cfg`.

## Colour Palette

| Element | Hex Code | Preview |
| ------- | -------- | ------- |
| **Terminal Green** | `#00FF00` | Track info, menu items |
| **Winamp Yellow** | `#E7D42F` | Menu active selection text, EQ peaks, volume label |
| **Winamp Orange** | `#D87818` | Volume progress rail fill |
| **Winamp Red** | `#D7443B` | EQ peak bars, low battery warning |
| **Electric Blue** | `#0000C6` | Menu selection bar |
| **Chassis Navy** | `#292941` | Panel interior surface |
| **Visualizer Navy** | `#171724` | Analyser background plate |
| **Deep Background** | `#050509` | Screen chassis rim |
| **Metallic Trim** | `#68687D` / `#39395A` | 3D bevels, borders, and frames |

## Compatibility & Notes

- **Target-Specific:** Designed and optimized exclusively for the **Hidizs AP80 Pro Max** (360 &times; 640 portrait screen).
- **Parser Validated:** Fully verified against Rockbox's native skin engine parser (`libskin_parser`) ensuring clean loading and rock-solid stability without failsafe fallbacks.
- **Self-Contained:** All necessary fonts and custom bitmaps are included in the package.

## Credits & Licence

- Theme design, UI layout, visualizer animation, and custom bitmaps are created for this theme.
- Bundled fonts are redistributed from the official Rockbox font package under their respective licenses (`.rockbox/fonts/COPYING-fonts.txt`).
- Winamp and Rockbox are trademarks of their respective owners. This is an open-source community tribute.
