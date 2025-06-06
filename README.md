# Deforestation Detection Using Landsat NDVI in Google Earth Engine (GEE)

This project detects deforestation by analyzing changes in vegetation using NDVI derived from Landsat 8 satellite imagery over two time periods.

## Project Overview

The workflow includes:
- Defining an Area of Interest (AOI).
- Loading Landsat 8 imagery for two different years (2015 and 2024).
- Calculating NDVI (Normalized Difference Vegetation Index) for each period.
- Computing NDVI change between the two periods.
- Identifying areas where NDVI has significantly decreased (indicating deforestation).
- Visualizing and exporting the detected deforestation map to Google Drive.

## Key Components

- **NDVI Calculation**: Uses Landsat bands (SR_B5 and SR_B4) to compute NDVI.
- **Change Detection**: Subtracts NDVI values between two time points.
- **Thresholding**: Deforestation is flagged where NDVI decrease is greater than 0.2.
- **Visualization**: 
  - NDVI 2015 and 2024
  - NDVI Change
  - Highlighted Deforestation Areas
- **Export**: Final deforestation layer is exported to Google Drive as a GeoTIFF.

## How to Use

1. Open [Google Earth Engine Code Editor](https://code.earthengine.google.com/).
2. Copy and paste the provided JavaScript code.
3. Modify the AOI coordinates if needed.
4. Click **Run** to execute.
5. Monitor the **Tasks** tab to export the deforestation map to Google Drive.

## Requirements

- A registered [Google Earth Engine](https://earthengine.google.com/) account.
- Internet access to use the GEE Code Editor.
- Basic understanding of NDVI and remote sensing concepts.

## Key Parameters

- **Area of Interest (AOI)**: Defined polygon for monitoring.
- **Time Periods**: 2015 and 2024.
- **Cloud Cover Filter**: Less than 20% for cleaner images.
- **Deforestation Threshold**: NDVI change less than -0.2.

## Output

- A GeoTIFF file (`Deforestation_Detection.tif`) highlighting deforested areas exported to your Google Drive.

## Author

© 2025 Okes Imoni
