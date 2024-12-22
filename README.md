# LCZ Classifier

LCZ Classifier is a project that automates the classification of Local Climate Zones (LCZ) using geospatial data. The process begins with satellite data acquisition through the Google Solar API and continues with a series of QGIS processing steps for LCZ classification.

## Features

- **Data Acquisition**: Web interface for downloading DSM, RGB and MASK tiles via Google Solar API
- **Automated Processing**: Series of Python scripts for QGIS that process data sequentially
- **LCZ Parameter Calculation**: Analysis of:
  - Sky View Factor
  - Aspect Ratio
  - Building Surface Fraction
  - Impervious/Pervious Surface Fraction
  - Height of Roughness Elements
  - Terrain Roughness Class
  - Surface Admittance
  - Surface Albedo
  - Anthropogenic Heat Output

## Prerequisites

- QGIS 3.x
- Python 3.x
- Google API Key for Google Solar API
- Python Libraries:
  - NumPy
  - Statsmodels
  - PyQt5

## Installation

1. Clone the repository
2. Open index.html in browser for the data download interface
3. Import Python scripts into QGIS

## Usage

### 1. Data Acquisition
- Open index.html
- Draw an area on the map
- Enter your Google API Key
- Generate API links and download tiles

### 2. QGIS Processing
Execute the scripts in the following order:

1. `00_import_raster_files.py`: Import downloaded raster files
2. `01_make_grid.py`: Create analysis grid
3. `02_make_buildings.py`: Extract buildings
4. `03_make_pervius_1.py`: Pervious surfaces analysis (part 1)
5. `04_make_pervius_2.py`: Pervious surfaces analysis (part 2)
6. `05_make_dtm.py`: Generate digital terrain model
7. `05_median_distance.py`: Calculate median distances
8. `05_mediana_altezze.py`: Calculate median heights
9. `06_make_h.py`: Calculate height of roughness elements
10. `07_aspect_ratio.py`: Calculate aspect ratio
11. `08_refine_albedo.py`: Refine albedo values
12. `09_rmsep.py`: Calculate and classify LCZs

## Project Structure

- `index.html`: Web interface for data download
- `scripts/`: Directory containing numbered Python scripts
- `docs/`: Additional documentation

## Contributing

Contributions are welcome! Please:

1. Fork the repository
2. Create a branch for your changes
3. Submit a pull request

## License

This project is distributed under the MIT license. See the `LICENSE` file for details.

## Authors

- [Your name]

## Acknowledgements

- Google Solar API
- QGIS Development Team
- Leaflet.js and contributors
