# Housing_Unit_Comparison
# Spatial Data Processing Workflow

## Overview

This project processes yearly spatial and tabular data from an enterprise GIS source and prepares a consolidated output for analysis.

The workflow extracts source datasets, applies time-based filtering, enriches records with coordinate information, links related datasets through shared identifiers, performs spatial matching against boundary layers, and produces a final analysis-ready dataset.

## What it does

- Connects to enterprise GIS data sources
- Filters records for a target year
- Exports selected spatial and tabular datasets into a local workspace
- Adds geographic coordinates to parcel-level features
- Joins parcel-related attributes to housing or unit-level records
- Converts tabular records into point features
- Assigns geographic boundary identifiers through spatial matching
- Handles a small number of manual exception cases
- Loads the final output into a dataframe for review or export

## Output

The result is a cleaned and joined dataset that combines:
- parcel-based location data
- unit or housing records
- geographic boundary assignments

This output can be used for comparison, reporting, and downstream spatial analysis.

## Requirements

- ArcGIS Pro
- Python
- `arcpy`
- `pandas`
- Access to the required enterprise GIS data sources

## Notes

This repository contains a generalized version of the workflow. Environment-specific connection files, schema names, paths, and other internal configuration details should be supplied locally and are not included here.
