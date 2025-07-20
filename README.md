# Flood Risk Detection Using Machine Learning and Remote Sensing

This project is part of a master's thesis focused on flood hazard mapping using satellite imagery and artificial intelligence. The objective is to identify flood-prone areas by extracting spatial features from geospatial data and training machine learning models to classify these regions accurately.

## Overview

Floods are one of the most devastating natural disasters, and accurate identification of high-risk zones is essential for disaster preparedness and urban planning. This project integrates remote sensing data (such as Sentinel-1 imagery and digital elevation models) with supervised machine learning algorithms to predict flood susceptibility.

## Data Sources

- **Sentinel-1 SAR imagery**
- **Digital Elevation Model (DEM30)**
- **Flood occurrence shapefiles**
- **Derived raster features** (e.g., NDWI, slope, water occurrence, aspect, distance to river, etc.)

All datasets are georeferenced and processed in GIS-compatible formats.

## Methodology

1. **Preprocessing & Feature Extraction**  
   Raster features are extracted at locations of known flood and non-flood points using shapefiles.

2. **Labeling**  
   Flood occurrence labels are assigned based on shapefile overlays.

3. **Data Preparation**  
   Data is cleaned, normalized, and split into training and testing sets.

4. **Model Training**  
   Multiple models are trained and compared, including:
   - Random Forest
   - XGBoost

5. **Evaluation**  
   Model performance is assessed using classification metrics (accuracy, precision, recall, F1-score) and visual tools such as confusion matrix and feature importance plots.

6. **Prediction & Mapping**  
   The trained model is applied on spatial rasters to generate flood hazard maps, which are visualized in GIS environments.

## Requirements

This project is implemented in Python. Major libraries used include:

- `rasterio`
- `geopandas`
- `numpy`
- `pandas`
- `scikit-learn`
- `xgboost`
- `matplotlib`

Please refer to `requirements.txt` for a full list of dependencies.

## Output

- Cleaned dataset with spatial features and flood labels  
- Trained machine learning models  
- Evaluation reports and plots  
- Flood susceptibility maps in GeoTIFF format

## Notes

This project was conducted as part of an academic research effort. All data has been processed and visualized responsibly. For further inquiries or academic collaboration, please contact the repository owner.

