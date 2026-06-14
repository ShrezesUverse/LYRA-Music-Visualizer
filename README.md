![LYRA — a planetarium for your sound](Source/brand/banner.png)

# LYRA

Is a runtime, GPU driven music visualizer for Windows that turns whatever you're listening to into an animation/visualization
> **LYRA is a private, fun made project. It is _not_ affiliated with, endorsed by, or sponsored by Spotify.**
> See [Disclaimer](#disclaimer) below.

---

## ✦ What it is

LYRA listens to your **system audio** — so it reacts to anything you play — and renders up to **one million GPU particles** that move with the music´s detected stems. Connect Spotify and it also knows the song's title, artist, and artwork, and recolors the whole scene to match each album.

It's a personal project, built for the joy of making something beautiful — Latest: ([PATCHNOTES-v0.2.0-ALPHA.md](PATCHNOTES-v0.2.0-ALPHA.md))

## ✦ Requirements

- **Windows 10/11, 64-bit**
- A **WebGPU-capable GPU** (developed on an NVIDIA RTX 5090; old GPUs can drop to a lower particle tier)
- **Spotify Premium** account — for the Spotify features (now-playing + per-album color). The visualizer itself reacts to system audio and works with any source.

## ✦ Spotify (Premium) set up (LYRA V1-V2)

LYRA will ask for an Client ID to connect your spotify client with it.
To get a Spotify Client ID, you need to create a developer application on the [Spotify for Developers Dashboard](https://developer.spotify.com/dashboard/).
1. **Log in**: Go to the Spotify for Developers site and log in with your standard Spotify account.
2. **Go to Dashboard**: Click on your profile icon in the top right corner and select [Dashboard](https://developer.spotify.com/dashboard/).
3. **Create an App**: Click the Create an app button. In the App Details: Fill in `LYRA` for App Name and Redirect URIs is `http://127.0.0.1:8888/callback`, accept the Terms of Service, and click Save.
4. **Find your Client ID**: Click on your newly created app from the [dashboard](https://developer.spotify.com/dashboard/), then click on Settings in the top right. Your Client ID will be visible right there.
Done!

## ✦ Running it

LYRA ships as a **portable executable**
1. Grab `LYRA.exe` from the `Release` folder.
2. Double-click it. (It self-extracts and runs.)
3. Play something, and if you want the Spotify extras, connect your Spotify account when/if prompted.

## ✦ Built with

- [Electron](https://www.electronjs.org/) + [electron-vite](https://electron-vite.org/) + TypeScript
- [three.js](https://threejs.org/) `r184` — **WebGPU renderer** + **TSL** (Three.js Shading Language), with GPU compute particles
- A custom AudioWorklet spectral-flux beat/onset detector

---
## ✦ Privacy

Your Spotify login stays on your machine´s AppData. The access token is stored locally and **encrypted with the OS keystore** — it is never bundled into the executable or sent anywhere except Spotify's own API. You are safe (:

More fun information and the controls list inside the repo `PATCHNOTES-v0.2.0-ALPHA.md`
--- 

## Disclaimer

LYRA is an **independent, non-commercial hobby project** made for fun. It is **not affiliated with, endorsed by, sponsored by, or connected to Spotify** in any way.

"Spotify" and the Spotify logo are trademarks of **Spotify AB**. LYRA uses the public Spotify Web API only to read now-playing metadata and album art for the signed-in user; it does not modify, redistribute, or stream Spotify content. All trademarks are the property of their respective owners.
```
I recommend the following songs to listen for the good visualisation
- https://open.spotify.com/track/65fPnec9ZIWi4YSMYOQXRm?si=32733bd86b5c4166 OUTTAHISMIND - Daniel Allan, Port London
- https://open.spotify.com/track/3Y1EvIgEVw51XtgNEgpz5c?si=1c4a5a3060f5472a Von Dutch - Charli xcx (aka Brat)
-
-
Enjoy
