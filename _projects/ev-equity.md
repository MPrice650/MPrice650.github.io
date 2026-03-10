---
title: "EV Charging Equity Analysis"
summary: "Geostatistical analysis identifying underserved communities in the Pacific Northwest's EV charging infrastructure rollout using accessibility modeling."
category: Spatial Analysis
thumb_class: analysis
tools: [Python, GeoPandas, OSRM, R, PostgreSQL]
year: 2023
role: Spatial Data Scientist
dataset: DOE AFDC, ACS 2022, OpenStreetMap
order: 3
github_url: https://github.com/yourgithub/ev-equity
---

## Overview

An equity-focused analysis of EV charging infrastructure access across Oregon and Washington, commissioned to inform a $40M federal infrastructure grant application.

## Methodology

Drive-time isochrones (5, 10, 20 minutes) were generated for all public Level 2 and DC Fast Chargers using the OSRM routing engine on OpenStreetMap data. These were intersected with census block groups and joined to ACS demographic variables. A composite Charging Access Score was derived using a weighted multi-criteria approach.

## Key Findings

Rural communities and tribal lands showed the starkest access gaps — 340,000 residents live more than 20 minutes from the nearest DC Fast Charger. Low-income urban neighborhoods are well-served by charger count but show high device-failure rates in operator maintenance records.

## Deliverables

Interactive StoryMap, technical report for DOE grant submission, and a Python package (released open-source) for replicating the isochrone-equity methodology in other states.
