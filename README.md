# 🎧 EchoCue

> A minimalist, Dockerized audio listener that reacts to in-game sounds in real time by triggering OBS events.

**EchoCue** monitors your system's audio output and detects specific in-game sounds (like extraction bells, deaths, or boss kills) using pitch/frequency pattern matching. When a match is detected, it uses the [OBS WebSocket API](https://github.com/obsproject/obs-websocket) to trigger overlays, scene changes, or stingers — automatically.

---

## 🚀 Features

- 🎙️ Real-time audio recognition via pitch and onset detection
- 🎮 Designed for games with no public API (*e.g. Hunt: Showdown*)
- 📦 Fully Dockerized — no GUI, no clutter
- 🔁 Trigger OBS scenes or effects automatically
- 🧩 Easily extendable with your own sound samples and match logic

---

## 📦 Installation

```bash
git clone https://github.com/yourname/echocue.git
cd echocue
docker build -t echocue .
