---
title: "Web/Desktop App Development - Bathymetry Tool"
summary: "A standalone Python application automating lake depth analysis via ArcPy. Features a custom PyQt5 GUI for loading depth shapefiles, selecting interpolation methods, and executing the full pipeline — outputting contour maps, raster surfaces, volume calculations, and a 3D ArcScene visualization. Deployable in office or field environments, and packageable as a custom ArcGIS Pro toolbox."
category: Python Development, GIS Automation, Spatial Analysis, GUI Design, ArcGIS Pro, 3D Visualization
thumb_class: carto
thumb_image: /assets/images/BathymertyMap/Bathymetric_Map.jpg
tools: [ArcGIS Pro, Python 3, ArcPy, Qt Designer, Remote Sensing, Spyder IDE]
year: 2023
role: Cartographer
dataset: NHD Plus v2, NLCD 2021, DEM 1/3 arc-second
order: 4
live_url: /bathymetry-portfolio.html
---

## Overview

A comprehensive print atlas produced for the Pacific Rivers Council, designed to accompany their annual watershed health report. All 48 maps were produced at CMYK print specifications for reproduction at A2 (420 × 594mm).

## Design Approach

Each map uses a custom hypsometric tint derived from a 10m DEM, with hand-tuned hillshading using multi-directional illumination. Typography follows an editorial newspaper grid, with basin names set in a condensed serif at varying optical sizes based on basin area.

## Technical Process

Watershed delineation and flow accumulation were computed in ArcGIS Pro using the NHD Plus v2 framework. Final cartographic refinement — symbol adjustment, typography, legend design, and color grading — was completed in Adobe Illustrator with linked data layers from QGIS.

## Reception

The atlas received the NACIS Student Competition (Professional Division) Gold Award and was featured in *Cartographic Perspectives* journal.
