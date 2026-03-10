---
title: "Amazon Deforestation Monitor"
summary: "Automated change-detection pipeline using Sentinel-2 time series to flag deforestation events in near real-time across the Brazilian Amazon."
category: Remote Sensing
thumb_class: remote
tools: [Google Earth Engine, Python, Sentinel-2, GEE JavaScript API]
year: 2024
role: Lead GIS Analyst
dataset: ESA Sentinel-2 MSI Level-2A
order: 2
github_url: https://github.com/yourgithub/amazon-monitor
---

## Overview

A near real-time monitoring system that detects forest cover change across 5.5 million km² of the Brazilian Amazon using bi-weekly Sentinel-2 imagery.

## Methodology

NDVI and EVI indices are computed from cloud-masked 10m composites. A pixel-wise statistical baseline is established from 2017–2020 imagery, and any deviation beyond 2.5 standard deviations triggers an alert. Alerts are spatially clustered, attributed to land tenure databases, and delivered via email digest and GeoJSON API.

## Results

The system detected over 2,400 discrete clearing events in its first operational year, with a 91% confirmation rate upon visual inspection. Mean alert latency is 11 days from initial clearing.

## Infrastructure

Fully serverless: Google Earth Engine handles all raster computation. A Cloud Functions pipeline manages alert generation and routing to a Firebase Realtime Database, with a Leaflet frontend consuming the alerts API.
