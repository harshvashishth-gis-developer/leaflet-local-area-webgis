# 🗺️ Madisonville Local Area WebGIS

### Interactive Web Mapping Application Using Leaflet.js, HTML, CSS, and JavaScript

**Developer:** Harsh Vashishth  
**Project Duration:** October 5–10, 2026  
**Study Area:** Madisonville, Kentucky, USA  
**Project Type:** WebGIS Development and Interactive Mapping  
**Technologies:** Leaflet.js | JavaScript | HTML5 | CSS3 | Esri Basemaps

---

## 🌐 Live WebGIS Application

**[Launch Interactive Madisonville WebGIS](https://harshvashishth-gis-developer.github.io/leaflet-local-area-webgis/)**

*The live application will be accessible after GitHub Pages has been enabled and deployed.*

## 📌 Project Overview

The **Madisonville Local Area WebGIS** is an interactive, browser-based geographic information system developed using Leaflet.js, JavaScript, HTML, and CSS.

The project demonstrates fundamental WebGIS concepts, including interactive map development, online basemap integration, geographic feature visualization, layer management, popup configuration, and responsive web interface design.

The application focuses on Madisonville, Kentucky, and includes sample point locations, a connecting line, and a demonstration study-area polygon.

This project was developed through a structured five-day learning workflow, progressing from a basic Leaflet map to a complete interactive WebGIS application.

**Note:** The vector features are illustrative practice geometries and do not represent verified roads, parcels, or official administrative boundaries.

---

## 🎯 Project Objectives

The primary objectives of this project were to:

1. Understand the fundamentals of WebGIS and interactive web mapping.
2. Develop an interactive web map using Leaflet.js.
3. Create and visualize point, line, and polygon features.
4. Integrate multiple Esri basemaps.
5. Organize geographic features using layer groups.
6. Implement interactive layer visibility controls.
7. Configure descriptive popups for spatial features.
8. Design a professional interface using HTML and CSS.
9. Create a map legend and information sidebar.
10. Integrate navigation tools, coordinate display, and a scale bar.
11. Prepare a complete WebGIS application for GitHub hosting and portfolio presentation.

---

## 🗺️ Final WebGIS Application

![Final Madisonville WebGIS](screenshots/Final_Madisonville_WebGIS.png)

The final application contains a custom-designed header, information sidebar, interactive map, map legend, basemap selector, overlay controls, and navigation tools.

### Key Features

**1. Interactive Map**

- Pan and zoom around Madisonville, Kentucky.
- Explore geographic features through clickable popups.
- View the study area using multiple basemaps.

**2. Multiple Basemaps**

The application integrates three Esri basemaps:

- Street Map
- Satellite Imagery
- Topographic Map

Users can switch between these basemaps using the Leaflet layer control.

**3. Geographic Features**

The application demonstrates three vector geometry types:

- **Points:** Sample locations represented by interactive circular markers.
- **Lines:** A demonstration connecting route.
- **Polygons:** An illustrative study-area boundary.

**4. Layer Management**

Users can independently show or hide:

- Point Locations
- Sample Route
- Study Area

**5. Interactive Popups**

Each geographic feature includes a popup displaying descriptive information.

**6. Custom Map Legend**

The sidebar legend identifies point locations, route geometry, and the study-area polygon using matching symbols.

**7. Navigation Tools**

- Map zoom controls
- Zoom to Study Area button
- Map scale bar
- Live latitude and longitude display

**8. Responsive Interface**

The application uses HTML and CSS to provide a structured layout with a map, information sidebar, and navigation tools.

---

## 📅 Project Development Workflow

The project was developed over five sequential learning stages.

### Day 1 — October 5, 2026

**Topic: Introduction to WebGIS and First Leaflet Map**

**Activities:**

- Introduction to WebGIS concepts.
- Understanding Leaflet.js and browser-based mapping.
- Creating a basic HTML webpage.
- Importing Leaflet CSS and JavaScript libraries.
- Initializing a map using `L.map()`.
- Setting map center coordinates and zoom level.
- Displaying an online Esri basemap.

**Outcome:** Created the first interactive Leaflet web map centered on Madisonville, Kentucky.

![Day 1 - First Leaflet Map](screenshots/Day1_First_Leaflet_Map.png)

### Day 2 — October 6, 2026

**Topic: Points, Lines, and Polygons**

**Activities:**

- Creating point markers.
- Assigning geographic coordinates.
- Adding interactive popup information.
- Creating polylines using `L.polyline()`.
- Creating polygons using `L.polygon()`.
- Understanding basic vector geometry visualization.

**Outcome:** Developed a local-area map containing point locations, a connecting line, and a demonstration polygon.

**Point Marker and Popup**

![Day 2 - Point Marker Popup](screenshots/Day2_Point_Marker_Popup.png)

**Point, Line, and Polygon Features**

![Day 2 - Vector Features](screenshots/Day2_Vector_Features.png)

### Day 3 — October 7, 2026

**Topic: Layers and Basemaps**

**Activities:**

- Understanding the difference between basemaps and overlays.
- Integrating multiple Esri basemaps.
- Organizing features using `L.layerGroup()`.
- Creating a layer-control interface.
- Switching between Street, Satellite, and Topographic basemaps.
- Enabling and disabling individual vector feature groups.

**Outcome:** Implemented interactive basemap selection and layer visibility controls.

![Day 3 - Layers and Basemaps](screenshots/Day3_Layers_Basemaps.png)

### Day 4 — October 8, 2026

**Topic: HTML, CSS, and WebGIS Interface Design**

**Activities:**

- Creating a custom webpage header.
- Designing an information sidebar.
- Adding a map legend.
- Applying CSS styling to the application.
- Improving the overall layout and readability.
- Introducing responsive design principles.
- Styling point, line, and polygon features.

**Outcome:** Transformed the basic Leaflet map into a structured WebGIS interface.

### Final Day — October 9–10, 2026

**Topic: Final Local Area WebGIS Development**

**Activities:**

- Consolidating previous mapping exercises.
- Refining the final application layout.
- Integrating a map scale bar.
- Implementing live coordinate display.
- Adding a Zoom to Study Area function.
- Finalizing interactive layer controls.
- Reviewing map symbology and popups.
- Preparing screenshots and documentation.
- Organizing the project for GitHub.

**Outcome:** Completed a portfolio-ready interactive WebGIS application demonstrating fundamental web mapping functionality.

---

## 🛠️ Technologies and Tools

| Technology | Purpose |
|---|---|
| Leaflet.js | Interactive mapping and geographic layer management |
| JavaScript | Map functionality, events, and navigation |
| HTML5 | Webpage structure and map container |
| CSS3 | Interface design, legend, and responsive layout |
| Esri Basemaps | Street, satellite, and topographic map visualization |
| Visual Studio Code | Code development and editing |
| GitHub | Project hosting and documentation |
| GitHub Pages | Static website deployment |

---

## 📍 Study Area

**Location:** Madisonville, Hopkins County, Kentucky, USA

**Approximate Map Center:**

- Latitude: 37.3281° N
- Longitude: 87.4989° W

The project uses a demonstration map centered on Madisonville.

The point, line, and polygon coordinates were created for WebGIS development practice and should not be interpreted as authoritative geographic datasets.

---

## ⚙️ Technical Workflow

### Step 1 — Initialize the Map

The Leaflet map is initialized using a geographic center and zoom level.

```javascript
var map = L.map('map').setView(
    [37.3281, -87.4989],
    13
);
```

### Step 2 — Add Basemaps

Esri tile services provide the background map layers.

```javascript
var streetMap = L.tileLayer(
    'https://server.arcgisonline.com/ArcGIS/rest/services/World_Street_Map/MapServer/tile/{z}/{y}/{x}',
    {
        maxZoom: 19,
        attribution: 'Tiles &copy; Esri'
    }
);
```

### Step 3 — Create Vector Features

Point, line, and polygon features are created using Leaflet geometry functions.

```javascript
L.circleMarker([37.3281, -87.4989]);

L.polyline([
    [37.3281, -87.4989],
    [37.3330, -87.4950],
    [37.3400, -87.4900]
]);

L.polygon([
    [37.3230, -87.5100],
    [37.3230, -87.5000],
    [37.3300, -87.4960]
]);
```

### Step 4 — Organize Geographic Layers

Related spatial features are organized into layer groups.

```javascript
var pointLayer = L.layerGroup([
    madisonvilleMarker,
    secondMarker
]);
```

### Step 5 — Implement Layer Controls

Leaflet's layer-control functionality allows users to select basemaps and manage overlay visibility.

```javascript
L.control.layers(
    baseMaps,
    overlayMaps,
    {
        collapsed: false,
        position: 'topright'
    }
).addTo(map);
```

### Step 6 — Develop the User Interface

HTML and CSS are used to create:

- A project header and title.
- A descriptive information sidebar.
- A custom map legend.
- Navigation controls.
- A responsive application layout.

### Step 7 — Add Interactive Navigation

JavaScript provides additional functionality, including:

- Coordinate tracking through Leaflet's `mousemove` event.
- Automatic zooming using `fitBounds()`.
- A map scale bar using `L.control.scale()`.

---

## 📂 Repository Structure

```text
leaflet-local-area-webgis/
│
├── index.html
├── README.md
│
├── daily-exercises/
│   ├── Day1_First_Leaflet_Map.html
│   ├── Day2_Vector_Features.html
│   ├── Day3_Layers_Basemaps.html
│   └── Day4_HTML_CSS_Legend.html
│
└── screenshots/
    ├── Day1_First_Leaflet_Map.png
    ├── Day2_Point_Marker_Popup.png
    ├── Day2_Vector_Features.png
    ├── Day3_Layers_Basemaps.png
    └── Final_Madisonville_WebGIS.png
```

The `index.html` file contains the final application.

The `daily-exercises` directory preserves the learning progression, while the `screenshots` directory documents the visual outputs.

---

## 🚀 How to Run the Project

### Option 1 — View Online

Once GitHub Pages is deployed, visit:

https://harshvashishth-gis-developer.github.io/leaflet-local-area-webgis/

### Option 2 — Run Locally

1. Download or clone the repository.
2. Open the project folder.
3. Locate `index.html`.
4. Open the file in a modern web browser.
5. Ensure an internet connection is available to load Leaflet and the Esri basemap tiles.

No backend server or database is required.

---

## 🧪 Application Testing

The application can be tested for:

- Successful basemap loading.
- Correct point, line, and polygon visualization.
- Functional feature popups.
- Basemap switching.
- Overlay visibility controls.
- Sidebar and legend display.
- Zoom functionality.
- Scale bar visibility.
- Live coordinate display.
- Responsive layout.

---

## 📚 Skills Developed

This project strengthened practical skills in:

- WebGIS fundamentals
- Interactive web mapping
- Leaflet.js development
- HTML and CSS
- JavaScript event handling
- Vector geometry visualization
- Cartographic symbolization
- Layer management
- Basemap integration
- Web interface design
- Technical documentation
- GitHub project organization

---

## ⚠️ Project Limitations

- Point, line, and polygon features are illustrative demonstration geometries.
- The sample route does not represent a verified navigable road.
- The study-area polygon is not an official administrative boundary.
- The application does not currently connect to a spatial database.
- Geographic features are defined directly in JavaScript.
- Basemap tiles require an internet connection and are subject to provider availability and usage conditions.
- The application is intended for educational and portfolio demonstration purposes.

---

## 🔮 Future Improvements

Potential future enhancements include:

1. Importing GeoJSON and other geographic datasets.
2. Integrating official local government GIS layers.
3. Adding a location search tool.
4. Creating a feature attribute table.
5. Implementing distance and area measurement tools.
6. Adding a basemap gallery.
7. Integrating GPS/geolocation functionality.
8. Connecting the application to GIS web services.
9. Adding thematic maps and spatial analysis results.
10. Improving mobile accessibility and performance.

---

## 👨‍💻 Author

**Harsh Vashishth**

M.S. Earth & Environmental Sciences  
GIS | Remote Sensing | Environmental Science | WebGIS

**GitHub Profile:**  
https://github.com/harshvashishth-gis-developer

**GIS Portfolio:**  
https://harshvashishth-gis-developer.github.io/

**Project Repository:**  
https://github.com/harshvashishth-gis-developer/leaflet-local-area-webgis

---

## 📄 Project Summary

The Madisonville Local Area WebGIS demonstrates the development of a browser-based interactive mapping application using open-source web mapping technologies.

Through progressive development exercises, the project integrates basemap services, spatial feature visualization, layer management, popups, custom interface styling, and interactive navigation.

The completed application provides a foundation for further development in WebGIS, spatial data visualization, and interactive geographic information systems.
