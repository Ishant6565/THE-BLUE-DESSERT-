# The Blue Desert

An offline, interactive clone of [The Blue Desert](https://thebluedesert.com/), an immersive WebGL storytelling experience by Adoratorio Studio.

The project preserves the original client-side runtime, including the animated loader, WebGL scenes, chapter navigation, custom cursor, scroll-driven transitions, atmospheric audio, responsive mobile gate, and interactive visual effects.

## Run locally

From the project directory, start the static server:

```powershell
python -m http.server 4173
```

Then open:

- Homepage: http://localhost:4173/
- Archive route: http://localhost:4173/archive-true/

The site is designed for a desktop browser. On smaller screens it keeps the original rotate-device experience.

## Project structure

- `index.html` - homepage application shell and SEO/social metadata
- `archive-true/index.html` - alternate route using the same interactive runtime
- `assets/` - bundled JavaScript, CSS, fonts, icons, and interface artwork
- `audio/` - ambient music, sound effects, and chapter voiceovers
- `images/` - chapter artwork and text-card graphics
- `svg/` - interface and navigation artwork
- `video/` - loader video
- `webgl/` - Draco decoder, models, HDR environment, and scene textures

## Verification

Both routes have been checked locally in desktop and mobile viewports. The runtime loads the WebGL canvas, custom cursor, loader, responsive mobile message, chapter navigation, audio assets, and scene assets without failed network requests.

## Attribution

This repository contains an offline copy of third-party creative work. The original content, artwork, code, music, and brand remain the property of their respective owners. This clone is intended for local study and reference.