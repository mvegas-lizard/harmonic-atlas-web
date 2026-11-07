# Third-party notices

## Original celestial artwork and mythological text

The sixteen illustrations under `art/myths/` were newly generated with the built-in image generation tool, with creative direction by mvegas. They are antique-inspired interpretations. Full prompts, asset hashes, and provenance are recorded in `art/myths/manifest.json`. They are included with this project's MIT distribution.

Myth summaries are original short paraphrases, not copied source passages. Selected traditions and source links appear in each story in the application. References include NASA Chandra constellation pages and Theoi's star-myth collection. Other cultural traditions remain distinct.

## HYG star positions and derived charts

The 107 selected star records and derived star-chart coordinates used in the application are adapted from **HYG v4.1**, by **David Nash / Astronomy Nexus**, under **Creative Commons Attribution-ShareAlike 4.0 International**. This data license is independent of the MIT code, original text, and illustrations.

- Source: https://github.com/astronexus/HYG-Database/blob/main/hyg/CURRENT/hygdata_v41.csv
- Catalog documentation: https://github.com/astronexus/HYG-Database/blob/main/hyg/README.md
- License: https://creativecommons.org/licenses/by-sa/4.0/
- Included notice: `licenses/HYG-STAR-DATA.txt`
- Changes: a 107-star subset, labels, brightness weights, and uniformly scaled stereographic chart coordinates (north up, east left), from J2000 right ascension and declination.

These adapted chart data are distributed under CC BY-SA 4.0. Connecting lines are authored atlas conventions; IAU constellation boundaries are not drawn. The Big Dipper is an asterism within Ursa Major; the Great Square of Pegasus includes Alpheratz in Andromeda. Plates are educational illustrations, not navigation charts. The original figure artwork is separate from the coordinate data.

## Salamander Grand Piano V3

Piano samples by **Alexander Holm**, licensed under **Creative Commons Attribution 3.0 Unported**.

- Original library: https://archive.org/details/SalamanderGrandPianoV3
- Source distribution: https://github.com/sfzinstruments/SalamanderGrandPiano
- Web MP3 rendering used here: https://tonejs.github.io/audio/salamander/
- License: https://creativecommons.org/licenses/by/3.0/
- Full consulted license text: `audio/LICENSE.txt`
- Per-file URLs, hashes, sizes, and processing notes: `audio/manifest.json`.

The included files are unmodified copies of 13 Tone.js-hosted MP3 renderings. Harmonic Atlas selects a small bank, repitches nearby samples at runtime, and applies playback gain, note duration, and optional room reverb. No endorsement by the sample author is implied. The sample license is independent of this project's code license.

## Fonts

- Inter, copyright The Inter Project Authors, SIL Open Font License 1.1. Local distribution through `@fontsource/inter`.
- Cormorant Garamond, copyright The Cormorant Project Authors, SIL Open Font License 1.1. Local distribution through `@fontsource/cormorant-garamond`.

Full notices are copied into `licenses/` and included in the production build.

## Runtime libraries

### MP3 encoding

`@breezystack/lamejs` 1.2.7 is distributed under LGPL-3.0. Its unmodified encoder, original notice, full LGPL/GPL texts and corresponding source archive are included in `vendor/lamejs-1.2.7/`. The module is loaded separately by the MP3 worker and can be replaced independently. See its [component notice](vendor/lamejs-1.2.7/NOTICE.md). This component retains its own license; original Harmonic Atlas code remains MIT, copyright mvegas.

Exported MP3 files carry an ID3 comment acknowledging the Salamander piano samples, Alexander Holm, their CC BY 3.0 license and source, and Harmonic Atlas as the application used to make the recording. The musical performance is not attributed to the application's author.

### Application libraries

React and React DOM (MIT), Tone.js (MIT), Tonal (MIT), Zod (MIT), and Lucide icons (ISC). Full top-level runtime notices are included in `licenses/`; generated bundles may also include notices for transitive code. Development tools retain the licenses in their installed packages and are not shipped as browser runtime dependencies.
