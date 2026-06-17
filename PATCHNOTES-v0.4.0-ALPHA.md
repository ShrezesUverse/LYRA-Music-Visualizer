# LYRA — v0.4.0 ALPHA · "Polyglot"

*A planetarium for your sound.*

The headline of this release: **LYRA now speaks your language.** The whole interface its been translated, the settings panel has been rebuilt from scratch, and the visuals detect the music far more better than before

---

## ✦ Languages

LYRA interface is now available in **6 languages**:

- **English / Spanish / german / French / Portugues / Italian**

It picks your **Windows language automatically** btw on first launch, and you can change any time in LYRA settings and in windows. Changing it updates the app instantly.

## ✦ Redesigned Settings

Settings gear menu is now available and you can change:

- **Particle count** - Low / Medium / High (250k / 500k / 1M)
- **Render resolution** - Performance / Balanced / Quality / Native. Lower it good for big or 4K screens and a much higher frame rate. However raise it to increase sharpnes of image
- **Fullscreen** - on/off, and LYRA now starts in fullscreen
- **Language** - the 6 options above


![The redesigned Settings panel](Source/0.4.0/NewUI/NewUI_01.png)

## ✦ better visuals

Reworked audio engine tracks onsets, tempo and drops with low latency, so impulses land on the beat. Kicks, builds and drops now getting detected as well.

## ✦ Audio that follows your output

- **Re-detect audio** If your audio doesnt get detected, that button might help. If not, go to windows settings, system, sound and switch to your default PC/desktop output and the to your prefered output.

## ✦ Also

- **No more sleep.** While audio is playing, LYRA keeps your PC awake so the screen never goes dark or sleeps.
- **Fullscreen support** via the render resolution control above.
- The debug overlay (`D`) now shows your **frame rate**.

## ✦ Controls

| Key | Action |
|-----|--------|
| `G` / `N` | (SCENES) Galaxy / Nebula |
| `1` / `2` / `3` | Quality tier ( in particles) — 250k / 500k / 1,000k |
| `R` | Re-acquire the audio device |
| `D` | **DEBUG** audio analysis overlay (now with fps) |
| `S` | **DEBUG** Shows track change transition on the scene |
| `I` | **DEBUG** Shows beat drop impulse on current scene |


## ✦ Notes

-`LYRA.exe` is a single self extracting portable. Download it, double-click, enjoy.
- Requires Windows 10 / 11, 64-bit, with a WebGPU-capable GPU and latest drivers.
- Now playing (title, artist, album art + per-album color) still works with **any** media app on Windows and no login and no Spotify Premium required anymore. Spotify is simply prioritised when it's open.

---

*Independent, non-commercial fun made project. Not affiliated with, endorsed by, or sponsored by Spotify or others
