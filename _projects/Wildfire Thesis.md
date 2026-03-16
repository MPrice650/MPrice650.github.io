---
title: "Wildfire Probability Analysis "
summary: "MA Thesis research mapping wildfire probability across Marin County, California. Built a multi-layer Boolean raster analysis in ArcGIS Pro across seven environmental variables, refined with WUI modeling, and validated against 222 MODIS thermal anomaly points and a century of historical fire boundaries. Linear regression in GeoDa identified soil moisture and land cover as the strongest predictors of fire occurrence, while exposing limitations in FEMA's National Risk Index as a spatial risk model."
category: Raster Analysis, Environmental GIS, Spatial Statistics, Thematic Cartography, Wildfire Risk Modeling
thumb_class: Remote Sensing
thumb_image: /assets/images/wildfire-maps/WildFire Risk Map.jpg
tools: [ArcGIS Pro, GeoDa, Python, MODIS, Cal Fire, FEMA]
year: 2024
role: Solo Developer & Analyst
dataset: USGS Landsat Collection 2
order: 1
github_url: https://github.com/yourgithub/urban-heat-island
live_url: /wildfire-portfolio.html
---

## Overview

This interactive dashboard lets users explore surface temperature differentials across five major U.S. metropolitan areas, revealing the urban heat island effect in striking visual detail.

## Methodology

Landsat 8 Band 10 (TIRS) imagery was processed to land surface temperature using a split-window algorithm. Cloud-masked composites were created for summer and winter seasons from 2018–2023. The thermal data was then joined to census tract boundaries to correlate temperature with socioeconomic indicators.

## Key Findings

Analysis revealed a consistent 4–8°C temperature differential between urban cores and surrounding vegetation. Low-income neighborhoods showed disproportionately high heat exposure, with 37% fewer tree canopy acres than high-income areas.

## Technical Stack

The frontend is built with Mapbox GL JS using custom terrain-interpolated raster tiles served from GeoServer. A Python/FastAPI backend handles dynamic queries against a PostGIS database containing 12 million temperature data points.
