# Project 3 - Calgary Building Permits Map

This project is a web-based interactive map that displays building permits issued in Calgary. It uses **Leaflet.js** for mapping, **Leaflet.markercluster** for clustering markers, and **OverlappingMarkerSpiderfier** to manage overlapping markers. The building permit data is fetched from the **City of Calgary Open Data Portal**.

## Features

- Interactive **Leaflet.js** map.
- Displays building permits issued in Calgary.
- **Date range selection** to filter permits.
- Uses **marker clustering** for better visualization.
- Handles **overlapping markers** using OverlappingMarkerSpiderfier.
- Fetches real-time data from the **Calgary Open Data API**.

## Technologies Used

- HTML, CSS, JavaScript
- [Leaflet.js](https://leafletjs.com/) (for maps)
- [Leaflet.markercluster](https://github.com/Leaflet/Leaflet.markercluster) (for marker clustering)
- [OverlappingMarkerSpiderfier](https://github.com/jawj/OverlappingMarkerSpiderfier-Leaflet) (for handling overlapping markers)
- [Flatpickr](https://flatpickr.js.org/) (for date range selection)
- [City of Calgary Open Data API](https://data.calgary.ca/)

## Installation & Usage

1. Clone this repository or download the project files.

   ```bash
   git clone https://github.com/Aayushh29/project3.git
   ```

2. Open the `index.html` file in your web browser.

3. Select a date range and click the **Search** button to fetch and display building permits.

## API Usage

This project uses the **City of Calgary Open Data API** to fetch building permit data. The API request format:

```
https://data.calgary.ca/resource/c2es-76ed.geojson?$where=issueddate >= 'YYYY-MM-DD' AND issueddate <= 'YYYY-MM-DD'
```

## How It Works

1. The **Leaflet map** initializes at Calgary's coordinates.
2. When a user selects a date range, an API request fetches building permit data.
3. The permits are displayed as markers on the map.
4. **Marker clustering** groups nearby markers.
5. **OverlappingMarkerSpiderfier** ensures that markers at the same location remain clickable.

## Dependencies

- [Leaflet.js](https://leafletjs.com/)
- [Leaflet.markercluster](https://github.com/Leaflet/Leaflet.markercluster)
- [OverlappingMarkerSpiderfier](https://github.com/jawj/OverlappingMarkerSpiderfier-Leaflet)
- [Flatpickr](https://flatpickr.js.org/)

## Notes

- Ensure you have an **internet connection** to load external scripts.
- The **City of Calgary API** must be available for data fetching.

---
