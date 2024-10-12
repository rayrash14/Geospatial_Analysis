This repository contains a project that demonstrates geospatial analysis using Python. It showcases how to visualize Points of Interest (POI) on an interactive map, retrieve data from OpenStreetMap (OSM) using the Overpass API, calculate distances between geographic locations, and present the results using folium.

# Overview
This project demonstrates:
- How to create, visualize, and analyze geospatial data.
- Fetching real-time POI data using OpenStreetMap and Overpass API.
- Calculating distances between manually defined POIs and OSM-retrieved POIs.
- Interactive mapping with markers and color-coded discrepancies based on proximity.

# Features
- **POI Data Creation:** Create a dataset of points of interest (POIs) with name, type, latitude, and longitude.
- **Geospatial Analysis:** Use geopandas for working with geospatial data and calculating distances.
- **OSM Data Retrieval:** Fetch POI data from OpenStreetMap using Overpass API.
- **Interactive Mapping:** Visualize POIs on a map with folium, with markers and pop-ups for additional info.
- **Discrepancy Visualization:** Color-code POIs based on calculated distance to nearby OSM POIs.

# Code Explanation
- **POI Data Setup:** Creates a sample dataset of POIs with name, type, latitude, and longitude.
- **GeoDataFrame Creation:** Converts the POI data into a GeoDataFrame for geospatial analysis.
- **Interactive Map Visualization:** Initializes a folium map and adds markers for each POI.
- **OSM Data Fetching:** Uses the Overpass API to retrieve nearby POIs from OpenStreetMap based on a specified radius.
- **Distance Calculation:** Calculates the distance between each original POI and the closest OSM POI.
- **Map with Discrepancies**: Updates the map to highlight POIs based on their proximity to nearby OSM data (green for close, red for far).

# Dependencies
The project requires the following Python libraries:

- pandas: For data manipulation.
- geopandas: Extends pandas for geospatial data.
- folium: For interactive map visualization.
- shapely: For handling and manipulating geometric shapes.
- requests: To fetch data from the Overpass API.
- osmnx: For OpenStreetMap data handling (optional but useful for more advanced geospatial tasks).
