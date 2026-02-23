# EcoRoute 🌿 — Carbon‑Smart Route Comparison

EcoRoute is a sustainability‑focused travel comparison web app that makes **carbon emissions visible before you commute**. Enter an origin + destination, view **multiple driving route alternatives on an interactive map**, and compare estimated emissions (and cost) across common transportation modes.

> Built for hackathon/demo use: fast, lightweight, and easy to run locally.

---

## ✨ Features

- **Origin → Destination** trip planning
- **Autocomplete address suggestions** (custom dropdown)
- **Multiple driving route alternatives** with:
  - Fastest route label
  - “Carbon‑optimal” route label (distance + traffic proxy)
  - Click a route card to **highlight it on the map**
- **Interactive map** using **Leaflet + OpenStreetMap tiles**
- **Emissions comparison** across modes:
  - 🚗 Gas Car
  - ⚡ Electric Vehicle
  - 🚌 Public Transit (per‑passenger)
  - 🚴 Cycling
  - 🚶 Walking
- Clear sustainability metrics:
  - Estimated CO₂
  - Green Score (0–100)
  - Estimated cost
  - CO₂ saved vs worst option
  - Trees/year offset estimate (rough)

---

## 🧱 Tech Stack

- **Frontend:** HTML + CSS + Vanilla JavaScript (single file)
- **Map rendering:** Leaflet + OpenStreetMap tiles
- **Route decoding:** `@mapbox/polyline`
- **Routing + autocomplete data:** Cloudflare Worker API (backend)
  - `GET /api/routes`
  - `GET /api/places`

---

## 🚀 Getting Started

### 1) Clone the repo
```bash
git clone <your-repo-url>
cd <your-repo-folder>
