# USA Transportation Noise Explorer

Interactive web map visualizing **transportation noise levels** from rail, road, and aviation sources across the United States (2020 data), built with ArcGIS Maps SDK for JavaScript 5.0 and Calcite Design System.

**[View Live App](https://garridolecca.github.io/transportation-noise-explorer/)**

![image](https://img.shields.io/badge/ArcGIS_JS-5.0-blue) ![image](https://img.shields.io/badge/Calcite-Design_System-purple) ![image](https://img.shields.io/badge/Data-2020-green)

## Features

- **Noise Visualization** - Color-coded raster layer (green 45 dB to red 124 dB) using a min-max stretch renderer
- **Click-to-Identify** - Click any location on the noise layer to see the exact decibel value with a human-readable description
- **Layer Controls** - Toggle layer visibility and adjust opacity via slider
- **Basemap Toggle** - Switch between dark and light basemaps
- **Coordinate Display** - Live lat/lon readout as you move the cursor
- **Noise Reference Guide** - Side panel with dB range descriptions and real-world comparisons
- **Responsive Dark Theme** - Calcite Design System dark mode with professional styling

## Data Source

**USA Transportation Noise - Rail, Road and Aviation (2020)**
- Source: [ArcGIS ImageServer](https://tiledimageservices.arcgis.com/P3ePLMYs2RVChkJx/arcgis/rest/services/USA_Transportation_Noise___Rail_Road_and_Aviation_2020/ImageServer)
- Pixel Type: 32-bit float (single band)
- Resolution: ~30 meters
- Range: 45 - 124 dB
- Spatial Reference: Web Mercator (WKID 3857)

## Tech Stack

- **ArcGIS Maps SDK for JavaScript 5.0** - Mapping, imagery tile layer, raster rendering
- **Calcite Design System** - UI shell, panels, blocks, sliders, switches, action bars
- **ImageryTileLayer** with `RasterStretchRenderer` and `MultipartColorRamp`

## Getting Started

No build step required. Open `index.html` in a browser or serve with any static file server:

```bash
npx serve .
```

## License

MIT
