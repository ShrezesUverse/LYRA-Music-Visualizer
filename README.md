![LYRA — a planetarium for your sound](Source/brand/banner.png)

# LYRA

Is a runtime, GPU driven music visualizer for Windows that turns whatever you're listening to into an animation/visualization
> **LYRA is a private, fun made project. It is _not_ affiliated with, endorsed by, or sponsored by Spotify.**
> See [Disclaimer](#disclaimer) below.

---

## ✦ What it is

LYRA listens to your **system audio** — so it reacts to anything you play — and renders up to **one million GPU particles** that move with the music´s detected stems. Connect Spotify and it also knows the song's title, artist, and artwork, and recolors the whole scene to match each album.

It's a personal project, built for the joy of making something beautiful — not a product.

## ✦ Requirements

- **Windows 10/11, 64-bit**
- A **WebGPU-capable GPU** (developed on an NVIDIA RTX 5090; old GPUs can drop to a lower particle tier)
- **Spotify Premium** account — for the Spotify features (now-playing + per-album color). The visualizer itself reacts to system audio and works with any source.

## ✦ Running it

LYRA ships as a **portable executable**
1. Grab `LYRA.exe` from the `Release` folder.
2. Double-click it. (It self-extracts and runs.)
3. Play something, and if you want the Spotify extras, connect your Spotify account when/if prompted.

## ✦ Built with

- [Electron](https://www.electronjs.org/) + [electron-vite](https://electron-vite.org/) + TypeScript
- [three.js](https://threejs.org/) `r184` — **WebGPU renderer** + **TSL** (Three.js Shading Language), with GPU compute particles
- A custom AudioWorklet spectral-flux beat/onset detector

```

## ✦ Privacy

Your Spotify login stays on your machine´s AppData. The access token is stored locally and **encrypted with the OS keystore** — it is never bundled into the executable or sent anywhere except Spotify's own API. You are safe (:

More fun information and the controls list inside the repo `PATCHNOTES-v0.2.0-ALPHA.md`
--- 

## Disclaimer

LYRA is an **independent, non-commercial hobby project** made for fun. It is **not affiliated with, endorsed by, sponsored by, or connected to Spotify** in any way.

"Spotify" and the Spotify logo are trademarks of **Spotify AB**. LYRA uses the public Spotify Web API only to read now-playing metadata and album art for the signed-in user; it does not modify, redistribute, or stream Spotify content. All trademarks are the property of their respective owners.

Enjoy
