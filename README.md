# NZ Regional Suitability Explorer

This is a web map that compares the 16 regions of New Zealand by rent and number of jobs. You can drag the arc control to change how important rent and jobs are to you, and the map, ranking list and popups will change at the same time.

This is my individual project for 158.888 IT Project at Massey University.
Author: Dengyu Zhang

## Files

- index.html: the web page
- regions.geojson: the processed data used by the web page
- data_processing.ipynb: Python notebook for cleaning, joining and normalising the data
- Data/raw: the original datasets
- Data/processed: files created by the notebook

## How to run

Web page: open the folder in VS Code, right-click index.html and choose "Open with Live Server". It needs a local server because the browser can't load the GeoJSON file from a file opened directly. It also needs internet to load Leaflet and the OpenStreetMap map. It works best on a desktop browser.

Notebook: you need pandas, geopandas and numpy. Run it in the main project folder. After running, copy Data/processed/regions.geojson to the main folder.

## Data sources

- Rental bond data (March 2026), Tenancy Services, CC BY 3.0 NZ
- Business Employment Data (December 2025 quarter), Stats NZ, CC BY 4.0
- Regional Council 2023 (generalised), Stats NZ, CC BY 4.0

This work is based on/includes Stats NZ's data which are licensed by Stats NZ for reuse under the Creative Commons Attribution 4.0 International licence.
Map tiles © OpenStreetMap contributors.
