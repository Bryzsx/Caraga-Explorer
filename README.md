# Caraga Explorer — Best Tourist Spots for You and Your Family

An interactive web map of family-friendly tourist spots in the Caraga Region (Region XIII), Philippines, built with Leaflet.js and GeoJSON.

## 🎯 Project Overview

This project was created for the **Platform Technologies / Web GIS** midterm exam (AY 2025–2026). It answers the question: *"Where should we take the family this weekend in Caraga?"*

## ✅ Requirements Checklist

### Core Requirements (60 points)

| # | Requirement | Status | Notes |
|---|-------------|--------|-------|
| 1 | **Tile Layer** | ✅ | OSM basemap + CartoDB Positron (Light) + CartoDB Dark Matter |
| 2 | **GeoJSON Layer** | ✅ | Real province boundaries from NAMRIA/PSA via GitHub |
| 3 | **Spot Popups** | ✅ | Rich popups with: spot_name, description, entrance_fee, best_season, family_friendly |
| 4 | **Hover Effect** | ✅ | Province boundaries highlight on mouseover with spot count |
| 5 | **Layer Control** | ✅ | Custom toggle for 4 categories + Day-Trip Route |
| 6 | **8+ Markers** | ✅ | 20 real tourist spots across Caraga |
| 7 | **Zoom to Feature** | ✅ | Click province to zoom, click marker to fly |
| 8 | **Deployed URL** | ⏳ | [TO BE DEPLOYED] |

### Bonus Stretch Goals (+9 points)

| Bonus | Feature | Status | Points |
|-------|---------|--------|--------|
| Family Day-Trip Route | LineString connecting 3 spots (Balanghai → Enchanted River → Siargao) | ✅ | +3 |
| Choropleth Styling | Provinces colored by number of tourist spots | ✅ | +3 |
| Search/Filter | Search bar to find spots by name, category, or description | ✅ | +3 |

## 🗺️ All 20 Tourist Spots Included

### 🏖️ Beaches & Islands (6 spots)
| Spot | Province | Coordinates | Entrance Fee |
|------|----------|-------------|--------------|
| Siargao Island | Surigao del Norte | 9.905°N, 126.067°E | Free |
| Britania Islands | Surigao del Sur | 8.678°N, 126.199°E | ₱50-100 |
| Sohoton Cove | Surigao del Norte | 9.600°N, 125.917°E | ₱200-300 |
| Mabua Pebble Beach | Surigao del Norte | 9.783°N, 125.483°E | Free |
| Cagwait White Beach | Surigao del Sur | 8.917°N, 126.483°E | ₱30-50 |
| Kabujuan Islet | Surigao del Norte | 9.517°N, 125.950°E | ₱150 |

### 💧 Waterfalls & Rivers (5 spots)
| Spot | Province | Coordinates | Entrance Fee |
|------|----------|-------------|--------------|
| Tinuy-an Falls | Surigao del Sur | 8.171°N, 126.229°E | ₱75 |
| Enchanted River | Surigao del Sur | 8.370°N, 126.338°E | ₱30 |
| Bega Falls | Agusan del Sur | 8.583°N, 125.917°E | ₱20-50 |
| Togonan Falls | Agusan del Norte | 9.582°N, 125.520°E | Free |
| Libuacan Cold Spring | Surigao del Sur | 8.450°N, 126.283°E | ₱20-30 |

### ⛰️ Mountains & Nature (6 spots)
| Spot | Province | Coordinates | Entrance Fee |
|------|----------|-------------|--------------|
| Agusan Marsh | Agusan del Sur | 8.317°N, 125.867°E | ₱100-200 |
| Lake Mainit | Agusan del Norte/Surigao del Norte | 9.433°N, 125.523°E | Free |
| Mt. Hilong-hilong | Agusan del Norte | 9.097°N, 125.705°E | Free |
| Del Carmen Mangrove Forest | Surigao del Norte | 9.867°N, 125.983°E | ₱100-150 |
| Bonsai Forest | Dinagat Islands | 9.950°N, 125.983°E | ₱50-100 |
| Laswitan Lagoon | Surigao del Sur | 9.083°N, 126.050°E | ₱20-50 |

### 🏛️ Heritage & Culture (5 spots)
| Spot | Province | Coordinates | Entrance Fee |
|------|----------|-------------|--------------|
| Balanghai Shrine Museum | Agusan del Norte | 8.949°N, 125.544°E | ₱20 |
| Butuan National Museum | Agusan del Norte | 8.949°N, 125.544°E | Free |
| San Salvador del Mundo Parish | Davao Oriental | 7.317°N, 126.567°E | Free |
| Pusan Point | Davao Oriental | 7.283°N, 126.583°E | ₱20-30 |
| Delta Discovery Park | Agusan del Norte | 8.950°N, 125.533°E | ₱200/₱100 |

## 📂 Project Structure

```
CaragaTourism/
├── index.html              # Main application (Leaflet.js + all features)
├── data/
│   ├── caraga-provinces-real.geojson  # Official NAMRIA/PSA province boundaries
│   └── caraga-provinces.geojson       # Backup/approximate boundaries
└── README.md               # This file
```

## 🛠️ Technologies Used

- **Leaflet.js** — Interactive map library
- **Leaflet.markercluster** — Marker clustering for better UX
- **Leaflet GeoJSON** — Province boundary rendering
- **Nunito Font** — Friendly, rounded typography
- **Material Symbols** — Icon set
- **Wikimedia Commons** — Real tourist spot images (Creative Commons licensed)

## 📊 Data Sources

### Province Boundaries
- **Source**: NAMRIA/PSA via [GitHub Repository](https://github.com/bendlikeabamboo/barangay-boundaries-repository/releases/download/v2026.4.13.0/provinces.geojson)
- **Coverage**: 5 Caraga provinces
  - Agusan del Norte (PH16002)
  - Agusan del Sur (PH16003)
  - Dinagat Islands (PH16085)
  - Surigao del Norte (PH16067)
  - Surigao del Sur (PH16068)

### Tourist Spot Coordinates
Verified from:
- Wikipedia
- Wikimapia
- ProjectLIGTAS
- DOT Caraga
- Local tourism office pages

### Tourist Spot Images
All images sourced from **Wikimedia Commons** (Creative Commons licensed):
- Siargao Island photos by various photographers
- Tinuy-an Falls photos from Wikipedia
- Enchanted River photos from Wikipedia
- Lake Mainit by Tim Dangerfield
- Cagwait White Beach by JasmineGoforth
- San Salvador del Mundo Church from Wikimedia Commons
- And more...

## 🚀 How to Run Locally

1. Clone or download this project
2. Open terminal in the project folder
3. Run a local server:

```bash
# Using Python
python -m http.server 8000   <------ i copy ni  i butang sa  first na terminal 

# Using Node.js
npx serve .         <---------- i copy ni sa pang duha na terminal 

# Using PHP
php -S localhost:8000
```

4. Open `http://localhost:8000` in your browser

## 🌐 Deployment

To deploy, upload to one of these free hosting services:

### GitHub Pages
1. Push to GitHub repository
2. Go to Settings → Pages
3. Select "main" branch
4. Your map will be at `https://yourusername.github.io/repo-name/`

### Netlify
1. Drag and drop the project folder to [netlify.com/drop](https://app.netlify.com/drop)
2. Get instant URL

### Vercel
1. Connect your GitHub repository
2. Deploy automatically

## 👥 Group Members

- [Member 1 Name]
- [Member 2 Name]
- [Member 3 Name]

## ⚠️ Known Issues

1. Some Wikimedia Commons images may load slowly on slow connections
2. Choropleth styling uses approximate point-in-polygon checks
3. Mobile responsive but optimized for desktop viewing

## 📝 Academic Integrity

This project was completed following the academic integrity guidelines:
- All code written by group members
- Tourist spot data researched from official sources
- Images sourced from Wikimedia Commons (Creative Commons)
- AI coding assistants used for code structure guidance

---

**Platform Technologies / Web GIS** · AY 2025–2026
