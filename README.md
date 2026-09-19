# aer-wds-calibration
Network Calibration via Automated Elevation Assignment- AER Regional Hydraulic Model

### Key Engineering Steps:

1. **Topographic Spatial Fusion:** Uses `rasterio` to read a 24-bit Digital Elevation Model (DEM) and directly samples terrain heights onto junction nodes.
2. **CRS Verification:** Formally verifies that both the EPANET coordinate model and the raster operate natively on the **WGS 84 / UTM Zone 30N projection (EPSG:32630)** to prevent spatial data degradation.

3. Technical Stack
* **WNTR & EPANET 2.2:** Hydraulic simulation modeling.
* **Rasterio:** Geospatial terrain extraction.
