# 🧭 Essentials Finder

A mobile-first web tool that helps travelers, residents, and anyone in an emergency **find critical services nearby** — hospitals, ATMs, police stations, fuel pumps, pharmacies, schools, colleges, and metro stations.

Built entirely with free, open-source tools. No paid APIs. No signup. No tracking.

🔗 **Live Demo:** [https://anuvrat03.github.io/essentials-finder/](https://anuvrat03.github.io/essentials-finder/)

---

## 🎯 The Problem

When you're in an unfamiliar place — or in an emergency — you need to find:

- 🏥 The **nearest hospital** in seconds
- 🏧 An **ATM** before your cash runs out
- 🚓 A **police station** when you feel unsafe
- ⛽ A **fuel pump** when your tank is empty
- 💊 A **pharmacy** when you're unwell
- 🏫 A **school** or 🎓 **college** when relocating
- 🚇 A **metro station** when commuting

Existing apps require sign-up, show ads, or hide results behind paywalls. This tool does **one thing well** — it finds what you need, right now, using open data.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🏥 **Hospitals & Clinics** | Nearby medical facilities in one tap |
| 🏧 **ATMs & Banks** | Cash points sorted by distance |
| 🚓 **Police Stations** | For safety and emergencies |
| ⛽ **Fuel Stations** | Petrol, diesel, and CNG pumps |
| 💊 **Pharmacies** | Chemists and medical stores |
| 🏫 **Schools** | Primary and secondary schools |
| 🎓 **Colleges & Universities** | Higher education institutions |
| 🚇 **Metro Stations** | Urban metro/rapid transit stops |
| 📍 **GPS-based search** | Uses your live location |
| 📊 **Distance-sorted list** | Nearest first — no scrolling needed |
| 🗺️ **Interactive map** | Tap any pin for details |
| 🧭 **One-tap directions** | Opens Google Maps navigation |
| 🔄 **6-server fallback** | Keeps working even when one server is busy |
| ⚡ **Instant category switch** | Tap a different category anytime — cancels old search cleanly |
| 💾 **Result caching** | Switched-back categories load instantly |
| 📱 **Mobile-first** | Built for phones — no app install needed |

---

## 🛠️ Tech Stack

Everything runs in the browser. No backend, no database, no server costs.

| Layer | Technology |
|---|---|
| **Hosting** | GitHub Pages (free) |
| **Map rendering** | [Leaflet.js](https://leafletjs.com/) — open-source map library |
| **Map tiles** | OpenStreetMap standard tiles |
| **Place data** | [Overpass API](https://overpass-api.de/) — queries the OSM database |
| **Geolocation** | Browser `navigator.geolocation` API |
| **UI** | Vanilla HTML, CSS, JavaScript |

---

## 🔍 How It Works

### 1. Location
The browser asks permission for your GPS location. Once granted, the tool draws a **10 km search radius** around you on the map.

### 2. Query
For the selected category, the tool builds an **Overpass QL query** like this:
