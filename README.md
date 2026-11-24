# obverse_lookboor
# OBVERSE — Interactive Techwear Lookbook Slider

A single-file, full-viewport fashion e-commerce lookbook experience for **OBVERSE**, featuring seamless clip-path wipe transitions, shoppable garment hotspots, live currency conversion, a hold-to-zoom magnifier lens, quick-view and bag drawers, search and index overlays, focus mode, and a contextual custom cursor.

---

## Features

- **Masked Wipe Transitions & Kinetic Typography**: Edge-to-edge `clip-path` wipe transitions with a vertical seam label, rolling digit reels, line-masked info swaps, and character-masked background wordmarks that auto-scale to fit the viewport.
- **Multiple Navigation Modes**: Navigate via arrow controls, bottom dot indicators, horizontal drag/swipe gestures, scroll wheel, keyboard shortcuts, or the full-screen look index.
- **Shoppable Hotspots & Quick View**: Frosted glass hotspot tags with automatic screen-edge flipping, inline size chips (`S`, `M`, `L`, `XL`), a quick-view drawer with 300% detail crop inspection, colour swatches, and accordion specs.
- **Bag & Fly-to-Bag Animation**: Add individual sizes, open quick view, or add an entire look with staggered fly-to-bag crop animations, quantity controls, free shipping threshold over $500 USD, and toast notifications.
- **Live Currency Converter**: Switch between **USD ($)**, **EUR (€)**, **GBP (£)**, and **JPY (¥)** with smooth `requestAnimationFrame` price interpolation across all visible prices and totals.
- **Hold-to-Zoom Magnifier Lens**: Press and hold (`200ms+`) on a model's subject area to inspect details at `2.4×` magnification following the pointer.
- **Archive Search & Index Overlays**: Filter all pieces live by name, code, colour, or collaboration in the top search panel, or browse all five looks in the 5-column index grid.
- **Fullscreen Focus Mode & Custom Cursor**: Toggle `body.fs` focus mode (`F` or nav button), with a custom cursor (and `?rec` recording mode support) on fine-pointer devices.

---

## Collaborations & Catalogue

| Look | Collaboration | Season | Pieces |
| :--- | :--- | :--- | :--- |
| **01** | Asker × KODA | AW26 | `AK 07 Tech Trench`, `AK 07 Strap Boot` |
| **02** | Vesper × RUNE | SS27 | `VR 03 Padded Parka`, `VR 03 Cargo Trouser`, `VR 03 Track Runner` |
| **03** | Morrow × TEKTON | AW26 | `MT 11 Utility Jumpsuit`, `MT 11 Field Boot` |
| **04** | Lumen × AISO | SS27 | `LA 05 Layered Coat`, `LA 05 Wide Trouser`, `LA 05 Cloud Boot` |
| **05** | Nord × HALE | AW26 | `NH 09 Shell Cape`, `NH 09 Pleat Trouser` |

---

## Controls & Shortcuts

| Input | Action |
| :--- | :--- |
| `←` / `→` or Scroll / Drag | Previous / Next look |
| `F` | Toggle fullscreen focus mode |
| `Esc` | Close active drawer or overlay |
| Hold (`200ms+`) on subject | Activate `2.4×` magnifier lens |

---

## Tech Stack

- **HTML5 & CSS3**: Custom properties (`--bg`, `--ink`, `--mute`, `--line`, `--blue`, `--tag`), `clip-path` animations, `backdrop-filter`, `clamp()` responsive typography, and an inline SVG `feTurbulence` grain overlay.
- **Vanilla JavaScript**: State management, `requestAnimationFrame` physics/lerp and currency counters, Web Animations API (`WAAPI`) fly-to-bag trajectories, pointer/wheel/keyboard event handling, and dynamic viewport layout/crop calculations.
- **Typography**: **Inter Tight** (weights `200`–`600`) via Google Fonts with system Helvetica/Arial fallbacks.

---

## Usage

1. Clone or download this repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/<your-repo>.git
   ```
2. Open `index.html` directly in any modern browser (or serve it with a local static server).
3. Append `?rec` to the URL (e.g., `index.html?rec`) to enable the larger recording-mode cursor and skip the intro loader.

---

## Project Structure

```text
.
├── index.html   # Complete single-file application (styles, markup, data, and scripts)
└── README.md    # Project documentation
```
