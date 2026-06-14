# LYRA — v0.2.0 ALPHA

*A planetarium for your sound.*

This is the second alpha. The first alpha (**v0.1.0**) had contained one scene — the **Nebula**. This was a stellar nursery that gets visualised ONLY with the bass stem of the sound, recolors to each album, and triggers a **Supernova** when the track changes. v0.2.0 keeps all of that and adds an entire second universe, plus a much better stem detection system and reduced latency from 8ßms to arraound 42ms.

---
LYRA is no longer one scene. v0.2.0 adds the **Supercluster** — spiral galaxy — and a live scene switcher.

- **Press `G`** for the Galaxy, **`N`** for the OLD Nebula. Switch any time; only the active scene gets loaede on your GPU.
- Both scenes share the same audio systems and sound and per-album color.

---

## ✦ The Galaxy update

Designed to look like a big spiral inspired by the **Barred Spiral galaxy**:

- **Voluminous dusty arms** — every star is pushed off the spiral by turbulent noise, so the arms read as billowing dust clouds with real body (the same trick that gives the Nebula its weight).
- **A warm bright core with a living vortex** — a swirling whirlpool where the two arms are getting started, powered by bass stems.
- **Debris** tumbling through the arms, and **grain**.
- **Sharper** — the core's glow is restrained so the dust stays crisp instead of blooming the whole frame soft.
- **Ongoing distortion** — A big wave gets created with an interwal off 17 seconds when the bass is loud enough.
- **Per-album color** — the galaxy takes on the colors of whatever's playing, just like the Nebula scene.

The Nebula has its Supernova. The Galaxy now has two of its own:

- **Track change Density Wave.** When the song changes, a luminous compression shell launches out from the core, pulses the whole galaxy, **pulls the background starfield a bit inward and erupts it back out**
- **Hard beat dropsImpulse Shockwave.** On a song's biggest drops (about **2–3 times per A song**), a fast shockwave ring blasts outward — through the galaxy disk *and* through the background stars.

---

## ✦ Audio engine upgrade

Got a revamp:

- **Fixed signal saturation.**
- **Lower latency.**
- **More to listen to.** LYRA now tracks **kick, snare, and hi-hat transients separately** (not just bass), which is what lets the hi-hats sparkle the stars in the background.

---

## ✦ OTHER

- **Discord Rich Presence.** LYRA shows what you're listening to (or "Idle in the planetarium") on your Discord profile, with the LYRA artwork — Have your Discord open while having LYRA open
- **Identity.** LYRA now has an app icon and an splash screen on launch.
- **Stability.** Fixed a GPU-memory leak.

---

## ✦ DEBUG and Controls

| Key | Action |
|-----|--------|
| `G` / `N` | **G**alaxy / **N**ebula |
| `1` / `2` / `3` | Quality tier (particles) — **250k** / **500k** / **1,000,000** |
| `S` | **DEBUG** Manually blast track-change transition (current scene) |
| `I` | **DEBUG** Manually blast Galaxy beat-drop impulse |
| `D` | **DEBUG** Toggle audio-analysis debug overlay |
| `R` | Reload the audio detection core (if audio gets an delay) |

---

## ✦ Notes

- Run — `LYRA.exe`

- **Windows x64**, requires a **WebGPU-capable GPU** (developed on an RTX 5090); quality levels switch with — press:
--(Lowest) `1` or `2` or `3` (Highest)

- **Your Spotify login stays on your machine** — the token is encrypted locally and is never baked into the executable.

- This is an **alpha**: expect rough edges, and the `S`/`I`/`D` keys are developer conveniences left in for tinkering.

---

*Built with three.js (WebGPU + TSL) on Electron.*
