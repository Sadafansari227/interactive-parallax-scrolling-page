# ELSEWHERE — An Interactive Parallax Journey

A responsive, cinematic parallax-scrolling experience for the Techfest Interactive Parallax Scrolling Page challenge.

## Local cinematic videos
Place the three supplied MP4s at these paths; the page references local files only for video:

- `assets/videos/mountains.mp4`
- `assets/videos/ocean.mp4`
- `assets/videos/desert.mp4`

After adding the MP4s, set the corresponding values in `assets/videos/availability.json` to `true`. They are currently `false` because no MP4 files were present in the supplied project. This prevents requests for missing videos while retaining the poster fallback.

Video sources are attached only while their landscape is near the viewport. The clips are muted, looping, inline and use `preload="metadata"` when activated; distant scenes are paused and unloaded. If a clip is unavailable or playback is blocked, its landscape poster remains visible. Add the three MP4 files before publishing or testing playback.

## Parallax and interaction
- Long, sticky, full-screen scenes keep each cinematic background in view while the visitor scrolls through each environment.
- Scroll position drives distinct, smoothly animated layer speeds: video backgrounds drift slowly while foreground ridges, waves and dunes move faster.
- Mountain scene: mountain video, sunlight, drifting clouds, layered ridges and atmospheric fog.
- Ocean scene: ocean video, wave layers, a glowing horizon and reflected light.
- Desert scene: desert video, overlapping dunes, atmospheric heat haze and drifting dust.
- Cinematic opening and closing sections, scroll progress indicator and active section navigation.
- Reveal-on-scroll typography, responsive mobile menu, reduced-motion support and poster fallbacks.

## Run locally
Serve the project directory over HTTP (for example, run `python -m http.server 8000` from the project directory and open `http://localhost:8000`). No build step or package installation is needed. An internet connection is required for poster images and Google Fonts. Videos are local.

## Publish with GitHub Pages
1. Create a repository named `interactive-parallax-page`.
2. Upload `index.html`, `README.md`, and the `assets/videos/` directory with all three MP4s, preserving the filenames above.
3. Open **Settings → Pages**.
4. Select **Deploy from a branch**, choose `main` and `/(root)`, then Save.
5. Wait for the Pages URL to appear and test all scenes by scrolling on desktop and mobile.
6. Submit the hosted link to the task.
