# Mapping-and-visualizing-factories-pollutant-data-in-Europe

This project is part of a wider one made along with Gabriel Meirinho, Luís Reis and Manuel Deus, where my part was to  present an analysis of air pollution and industrial facility data across EU countries through three interactive visualizations.

---

## Table of Contents

- [Overview](#overview)
- [Visualizations](#visualizations)
  - [1. Interactive Radar Chart](#1-interactive-radar-chart)
  - [2. Emissions Over Time with Facility Data](#2-emissions-over-time-with-facility-data)
  - [3. Interactive Map of Facilities and Nearby Air Quality Stations](#3-interactive-map-of-facilities-and-nearby-air-quality-stations)
- [Data Files Used](#data-files-used)
- [Libraries Used](#libraries-used)
- [Outputs Generated](#outputs-generated)
- [Notes](#notes)
- [License](#license)

---

## Overview

The notebook explores two related datasets:

- **Air quality station measurements**
- **Industrial facility emissions**

It combines these datasets to compare pollution levels, emissions trends, and geographic proximity between stations and facilities.

---

## Visualizations

### 1. Interactive Radar Chart

This visualization compares average pollution indicators across EU countries using a radar chart for each country.

It covers:

- PM2.5
- NO2
- O3
- AQI

The values are normalized so countries can be compared on the same scale, while the original measurements are still shown in the chart.

---

### 2. Emissions Over Time with Facility Data

This section builds a Dash dashboard that lets the user compare emissions over time by country and pollutant.

The dashboard includes:

- a country selector
- a pollutant selector
- a switch between total emissions and average emissions per facility
- a statistics table with yearly values

---

### 3. Interactive Map of Facilities and Nearby Air Quality Stations

This visualization uses Folium to map air quality stations and nearby industrial facilities.

It:

- plots stations and facilities on an interactive map
- groups facilities by reporting year
- highlights facilities within 1 km of a station
- saves the final map as an HTML file

---

## Data Files Used

- `station_measurements_concat.csv`
- `facilities/facilities_cleaned.csv`

---

## Libraries Used

- `pandas` – data manipulation and analysis
- `numpy` – numerical operations
- `matplotlib` – plotting and visualisation
- `dash` – interactive dashboard framework
- `plotly` – interactive charts
- `folium` – interactive map visualisation
- `geopy` – geocoding and distance calculations
- `branca` – colour mapping for Folium

---

## Outputs Generated

- `all_countries_pollution_radar_charts.png` – radar charts for all countries
- `stations_facilities_1km_by_year.html` – interactive map showing stations and facilities within 1 km

---

## Notes

- The notebook is meant to be run cell by cell.
- The Dash visualizations run on port `8051`.
- The dataset files must be available at the paths used in the notebook.

---
