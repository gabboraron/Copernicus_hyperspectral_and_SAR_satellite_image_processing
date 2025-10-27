# Copernicus Hyperspectral and SAR Satellite Image Processing

Workshop notes and Jupyter notebooks for Earth Observation data processing, focusing on Copernicus satellite missions, SAR (Synthetic Aperture Radar) data, and hyperspectral image analysis.

## About This Repository

This repository contains my personal notes, code examples, and Jupyter notebooks from the **ESA Earth Observation (EO) Workshop** covering:

- **Copernicus Data**: Understanding and accessing Copernicus program data, including Sentinel missions
- **SAR Processing**: Working with Synthetic Aperture Radar data for remote sensing applications
- **Hyperspectral Image Processing**: Analyzing multispectral and hyperspectral imagery for earth observation

## Repository Structure

```
├── notebooks/
│   ├── copernicus_data/       # Notebooks about Copernicus program and Sentinel missions
│   ├── sar_processing/         # SAR data processing and analysis notebooks
│   ├── hyperspectral_processing/  # Hyperspectral imaging notebooks
│   └── examples/               # Example workflows and case studies
├── LICENSE                     # MIT License
└── README.md                   # This file
```

## Getting Started

### Prerequisites

To run the Jupyter notebooks in this repository, you'll need:

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- Common Python libraries for geospatial data processing:
  - NumPy
  - Matplotlib
  - GDAL/Rasterio (for geospatial data)
  - Sentinel data processing libraries (as needed)

### Theory
- [Senitnel 1](https://sentinels.copernicus.eu/copernicus/sentinel-1) - SAR
    - Monthly mosaics with terrain flattering
    - no swath edges, reduced speckle
    - high applicability for agriculture
    - 2020-2024
- Sentinel 2-3 for agriculture
  - Sentinel 2  ~ 5 day revisit
  - Sentinel 3  - twice daily
    - algal pigment
    - CDM absoption
    - calibrated NDVI 
- Sentinel 4 for ocean observation
- Sentinel 5 - most optical bands; daily

#### CCM
APIs:
+ Catalogue API -> return list of datasets
+ Visualisation(OGC) -> returns a map
+ process (instant batch) -> returns raster product
+ statistical -> returns calculation results
+ bring your own data -> Your own data visualized or merged

STAC catalogue:
- direct download
- S3 paths

[OpenEO](https://openeo.org/)

More:
- https://documentation.dataspace.copernicus.eu
- https://www.youtube.com/@copernicusdataspaceecosystem
- https://land.copernicus.eu/en
- https://github.com/eu-cdse/copernicus-browser


#### CRMS
- https://land.copernicus.eu/en/products/high-resolution-layer-forests-and-tree-cover/forest-type-2018-raster-10-m-100-m-europe-3-yearly

### Installation

1. Clone this repository:
```bash
git clone https://github.com/gabboraron/Copernicus_hyperspectral_and_SAR_satellite_image_processing.git
cd Copernicus_hyperspectral_and_SAR_satellite_image_processing
```

2. Set up a Python virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install Jupyter and required libraries:
```bash
pip install jupyter numpy matplotlib
# Additional libraries can be installed as needed for specific notebooks
```

4. Launch Jupyter Notebook:
```bash
jupyter notebook
```

## Notebook Topics

### Copernicus Data
- Introduction to Copernicus program and Sentinel missions
- Data access and download methods
- Data formats and structure
- Working with different Sentinel satellites (Sentinel-1, 2, 3, etc.)

### SAR Processing
- SAR technology fundamentals
- Sentinel-1 SAR data processing
- Preprocessing and calibration
- SAR applications (change detection, land cover mapping, etc.)

### Hyperspectral Processing
- Hyperspectral vs multispectral imaging
- Spectral signatures and analysis
- Classification techniques
- Processing workflows and best practices

## Data Sources

- **Copernicus Open Access Hub**: https://scihub.copernicus.eu/
- **Copernicus Data Space Ecosystem**: https://dataspace.copernicus.eu/
- **ESA Earth Online**: https://earth.esa.int/

## Resources

### Official Documentation
- [Copernicus Programme](https://www.copernicus.eu/)
- [ESA Sentinel Online](https://sentinels.copernicus.eu/)
- [Sentinel-1 Documentation](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-1)
- [Sentinel-2 Documentation](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-2)

### Learning Resources
- [ESA STEP (Sentinel Toolbox)](http://step.esa.int/)
- [Copernicus Training Materials](https://www.copernicus.eu/en/opportunities/education/training-materials)
- 

## Contributing

This is a personal learning repository, but suggestions and corrections are welcome! Feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- European Space Agency (ESA) for the Earth Observation workshop
- Copernicus Programme for providing open access to satellite data
- The Earth Observation community for excellent tools and documentation

## Contact

**Author**: Burián Sándor  
**Repository**: https://github.com/gabboraron/Copernicus_hyperspectral_and_SAR_satellite_image_processing

---

*Note: This repository is continuously updated as I progress through the workshop materials and expand my knowledge of Earth Observation data processing.*
