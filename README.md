# Geospatial Flood Assessment

This repository contains a comprehensive geospatial analysis pipeline for assessing flood impacts using various datasets and machine learning clustering techniques. The outputs include interactive maps, GeoJSON files, and raster visualizations.

## Key Concepts

This project uses advanced geospatial techniques and clustering algorithms to analyze flood impacts effectively. Key concepts include

- **Normalized Difference Vegetation Index (NDVI)**: Measures vegetation health by comparing the difference between near-infrared (vegetation reflects strongly) and red light.
- **Normalized Difference Water Index (NDWI)**: Highlights water bodies by analyzing the difference between green and near-infrared light.
- **Normalized Difference Built-up Index (NDBI)**: Detects built-up areas by analyzing the difference between short-wave infrared and near-infrared light.
- **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**: A machine learning algorithm that identifies dense regions in the dataset as clusters, making it suitable for identifying flood-affected zones.
- **HDBSCAN (Hierarchical Density-Based Spatial Clustering of Applications with Noise)**: An extension of DBSCAN that provides more robust clustering by building a hierarchy of density-based clusters and extracting the best possible grouping.

## Methodology

The analysis workflow includes:

1. **Data Preprocessing**: Input data such as satellite imagery and geospatial layers are processed to compute indices like NDVI, NDWI, and NDBI.
2. **Clustering Algorithms**:
   - DBSCAN: Identifies dense areas impacted by floods.
   - HDBSCAN: Hierarchical clustering for better cluster definitions.
3. **Cluster Severity Analysis**: Calculates severity metrics for clusters.
4. **Visualization**:
   - Generates GeoJSON and TIF outputs for mapping.
   - Produces interactive visualizations for detailed insights.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/geospatial-flood-assessment.git
   ```
2. Install dependencies for Jupyter Notebook:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook geospatial-flood-assessment.ipynb
   ```
4. Explore the results using the provided TIF, GeoJSON, and HTML files.

## Outputs

- **Raster Outputs**: Visualize changes in NDVI, NDWI, and NDBI, along with flood clusters.
- **Interactive Maps**: Explore flood impacts interactively via HTML files.
- **GeoJSON Files**: Use in GIS platforms for further analysis.

## Dependencies

- Python 3.8+
- Jupyter Notebook
- GeoPandas
- Rasterio
- Scikit-learn
- HDBSCAN
- QGIS (optional for QGZ files)

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss changes.

## Acknowledgments

- Satellite imagery and data sources.
- Open-source libraries and tools used in this analysis.

