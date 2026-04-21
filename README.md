# 🗺️ MALANG.HIDDEN - Discover the Unseen

> An interactive dark map explorer for uncovering hidden cafes, restaurants, bars, and spots in Malang, East Java.

![Static Badge](https://img.shields.io/badge/status-live-00ff9d?style=flat-square)
![Static Badge](https://img.shields.io/badge/data-OpenStreetMap-blue?style=flat-square)
![Static Badge](https://img.shields.io/badge/built%20with-HTML%20%2F%20CSS%20%2F%20JS-orange?style=flat-square)
![Static Badge](https://img.shields.io/badge/deploy-GitHub%20Pages-181717?style=flat-square&logo=github)

---

## ✨ Features

- **Live Data** Fetches real-time location data directly from OpenStreetMap via Overpass API. No database needed.
- **Interactive Map** Built with Leaflet.js, dark-themed with cyberpunk tile filter. Markers are color-coded by category.
- **Dark / Light Mode** Smooth animated theme toggle with preference saved to localStorage.
- **Category Filters** Filter by Cafe, Restaurant, Bar, Spot, or Park instantly.
- **Search** Real-time search across location names and addresses.
- **Location Detail Panel** Click any marker or card to reveal coordinates, category, WiFi info, opening hours, and a direct link to Google Maps.
- **My Location** Jump to your current GPS position on the map.
- **Coordinate Tracker** Live lat/lng display as you move your cursor across the map.
- **Zero Backend** Pure static site. No server, no database, no maintenance.

---

## 🖥️ Preview

| Dark Mode | Light Mode |
|-----------|------------|
| Cyberpunk dark map with glowing markers | Warm beige palette with natural map tiles |

---

## 🚀 Getting Started

### Run Locally

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/malang-hidden.git

# Open in browser — no build step needed
cd malang-hidden
open index.html
```

Or just drag `index.html` into your browser.

### Deploy to GitHub Pages

1. Push the repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `Deploy from a branch` → `main` → `/ (root)`
4. Your site will be live at:

```
https://YOUR_USERNAME.github.io/malang-hidden
```

---

## 🛠️ Tech Stack

| Tech | Usage |
|------|-------|
| HTML / CSS / JS | Core — no framework, no build tools |
| [Leaflet.js](https://leafletjs.com/) | Interactive map rendering |
| [OpenStreetMap](https://www.openstreetmap.org/) | Map tile provider |
| [Overpass API](https://overpass-api.de/) | Live POI data for Malang |
| [Google Fonts](https://fonts.google.com/) | Syne (display) + Space Mono (UI) |
| GitHub Pages | Hosting |

---

## 📁 Project Structure

```
malang-hidden/
└── index.html      # Entire app — single file, zero dependencies to install
```

---

## 🗂️ Data Source

All location data is fetched live from **OpenStreetMap** using the Overpass API. The query covers the Malang bounding box and pulls:

- `amenity = cafe`
- `amenity = restaurant`
- `amenity = bar / pub`
- `tourism = attraction / viewpoint`
- `leisure = park`

Only nodes with a `name` tag are shown. Data updates automatically as OSM contributors add and edit locations.

---

## 🎨 Design

- **Dark mode**: Deep navy/black with `#00ff9d` accent — cyberpunk terminal aesthetic
- **Light mode**: Warm `#f0ede8` beige with `#00915a` accent — clean and readable
- **Typography**: [Syne](https://fonts.google.com/specimen/Syne) for display + [Space Mono](https://fonts.google.com/specimen/Space+Mono) for UI
- **Map**: Dark mode applies `invert + hue-rotate` CSS filter to OSM tiles for a night-map look

---

## 📌 Roadmap

- [ ] Bookmark / save favorite locations
- [ ] Share a location via URL
- [ ] User-submitted hidden gems (via GitHub Issues as backend)
- [ ] Mobile-responsive layout
- [ ] Distance from current location

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

<div align="center">

Crafted with precision by **Agus Satria Adhitama**  
Malang, East Java 🌋

</div>
