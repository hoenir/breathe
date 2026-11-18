# Unfolding Star

A full-screen breathing exercise. A single line folds into a star as you breathe in and unfolds as you breathe out. Inhale, hold, exhale and rest durations are adjustable.

Live app: https://sandervandecruys.be/breathe/

## Heart rate

Connect any sensor that broadcasts the standard Bluetooth Heart Rate Profile (Fitbit Air via Google Health → Connections → Share heart rate, chest straps, many watches). Needs Chrome or Edge on Android, Windows or Mac; iPhone browsers have no Web Bluetooth.

- **Breath swing**: how far heart rate rises and falls within each breath. Works with bpm-only bands such as the Fitbit Air.
- **Before & after**: resting heart rate measured for 1–2 minutes before and after the session.
- **HRV (RMSSD)**: only with sensors that send beat-to-beat intervals, such as a Polar H10.

## Install on a phone

- **Android (Chrome)**: open the live app, then menu → *Install app* (or *Add to Home screen*).
- **iPhone (Safari)**: Share → *Add to Home Screen*. Breathing works; heart rate does not.

## Run locally

```bash
python -m http.server 8765 --directory app
```

Open http://localhost:8765. Add `?demo=air` to simulate a bpm-only band.

`breathe.html` is the original single-file prototype.
