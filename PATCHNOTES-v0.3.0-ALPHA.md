# LYRA — v0.3.0 ALPHA · "No Login"

*A planetarium for your sound.*

The headline of this release: **LYRA no longer needs a Spotify login.** The whole Spotify Web API has been removed and replaced with my Windows runtime stuff and audio tracking feed Windows already provides. It just works — for everyone. Yaay, we happy. NO Premium is needed.

---

## ✦ Spotify

Previous builds asked every user to create their own Spotify developer app, paste a Client ID, and set a redirect URI and, after Spotify's Feb 2026 API changes, also required **Spotify Premium** and capped each app at ~5 users. That's gone.

LYRA now reads the current track straight from **Windows System Media Transport Controls (SMTC)** the same source as the little media popup on your volume flyout.

- **No login. No Premium. No developer app. No user limit.**
Also...
— if Spotify is open, it's always what's shown.
— if Spotify is closed, LYRA shows whatever else is playing (a browser, Apple Music, anything).
- Title, artist, **album art**, and the per album color theming all work exactly as before just without the hoops. Ill figure something out.

Your now-playing info never leaves your machine.

## ✦ details

- If you are a spotify PREMIUM user, you should consider to download V2/V1 for now.

## ✦ Controls

| Key | Action |
|-----|--------|
| `G` / `N` | Galaxy / Nebula |
| `1` / `2` / `3` | Quality tier (particles) — 250k / 500k / 1,000k |
| `S` | **DEBUG** Fire the current scene's track-change transition |
| `I` | **DEBUG** Fire the Galaxy beat-drop impulse |
| `D` | **DEBUG** Toggle the audio-analysis debug overlay |
| `R` | **DEBUG** Re-acquire the audio device |

## ✦ Notes

- **Portable** — `LYRA.exe` is a single self-extracting file. Just double click and enjoy, ok?
- **Windows 10 / 11, 64-bit**, WebGPU capable GPU is required.
- Now-playing works with **any** media app on Windows; Spotify is simply prioritized when present.

---

*Independent, non-commercial hobby project. Not affiliated with, endorsed by, or sponsored by Spotify. "Spotify" is a trademark of Spotify AB.*
