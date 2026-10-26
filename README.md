# Nocturne Pointillist Water

A dark, interactive WebGL ocean wallpaper for **Lively Wallpaper**. The scene combines a pointillist night sky and liquid-glass water with marine life, a dot-matrix clock, and an `@saj` watermark. It is designed as a self-contained `index.html` with no external runtime dependencies.

## Features

- Animated, layered ocean waves rendered in a pointillist style
- Mouse interaction for water splashes and subtle movement across the scene
- Fish, bubbles, jellyfish, and seagulls
- System-audio reactivity when run through Lively Wallpaper
- Dot-matrix clock and `@saj` watermark
- Responsive full-screen layout
- Lively customization sliders for audio sensitivity, sea-life density, and splash strength

## Use with Lively Wallpaper

1. Keep `index.html`, `LivelyInfo.json`, and `LivelyProperties.json` together in the same folder.
2. In Lively Wallpaper, add a web wallpaper and browse to that folder's `index.html`.
3. Open the wallpaper's **Customize** settings to adjust the available sliders.
4. Enable audio capture in Lively if you want the scene to react to system audio. The wallpaper's Lively configuration requests audio with the `--audio` argument.

In a regular browser, the animation and mouse interaction work, but Lively's system-audio feed is not available, so audio-driven effects remain idle. Browser support and performance depend on the device and GPU.

## Customization

The Lively controls are declared in `LivelyProperties.json`:

| Setting | Range | What it changes |
| --- | ---: | --- |
| Audio Sensitivity | 0–200% | Strength of audio-driven effects |
| Sea Life Density | 0–100% | Amount of fish, jellyfish, and seagulls |
| Splash Strength | 0–200% | Strength of mouse-driven water interaction |

The wallpaper title, entry file, and audio argument are configured in `LivelyInfo.json`.

## Project files

- `index.html` — complete wallpaper implementation
- `LivelyInfo.json` — Lively wallpaper metadata and audio launch argument
- `LivelyProperties.json` — Lively customization settings

## Development note

This project was **vibe-coded**: it was created through iterative natural-language prompting with AI assistance. The implementation has been revised through browser testing, but AI-generated code can still contain bugs and has not necessarily received a comprehensive security, accessibility, or cross-device review. Contributions, testing, and careful review are welcome.
