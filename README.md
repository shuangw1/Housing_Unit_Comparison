# Housing Unit Spatial Data Pipeline

## Overview

Built an automated geospatial data pipeline that transforms yearly enterprise GIS datasets into a standardized, analysis-ready housing dataset.

The workflow integrates parcel geometry, housing-unit records, coordinate data, and administrative boundary assignments into a single reproducible output. It reduces manual GIS processing, improves consistency across reporting years, and supports downstream analytics, visualization, and operational decision-making.

## Key Capabilities

* Connects to enterprise spatial and tabular data sources
* Filters and processes records for a configurable reporting year
* Extracts required datasets into a structured local workspace
* Generates geographic coordinates for parcel-level features
* Joins parcel attributes with housing and unit-level records
* Converts tabular records into spatial point features
* Assigns administrative and reporting-area identifiers through spatial joins
* Applies validation rules and resolves limited exception cases
* Loads the consolidated output into a Pandas DataFrame for quality review, analysis, or export

## Business Impact

The pipeline replaces a multi-step manual workflow with a repeatable and scalable process. It enables teams to:

* Produce consistent annual housing datasets
* Reduce data preparation time and human error
* Compare housing trends across years and geographic areas
* Support reporting, market analysis, planning, and location-based decision-making
* Reuse the workflow across different datasets and enterprise GIS environments

## Output

The final dataset combines:

* Parcel-based location and coordinate data
* Housing or unit-level attributes
* Geographic boundary and reporting-area assignments

The resulting table is ready for statistical analysis, dashboard development, mapping, and other downstream spatial workflows.

## Technology Stack

* Python
* ArcPy
* Pandas
* ArcGIS Pro
* Enterprise GIS databases

## Repository Notes

This repository contains a generalized and reusable version of the production workflow. Organization-specific database connections, schema names, file paths, credentials, and internal configuration settings are intentionally excluded and must be configured locally.
