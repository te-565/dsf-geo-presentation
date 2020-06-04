# dsf-presentation
Code and useful stuff to support my Data Science Festival presentation on 04/04/2020.

## Manual Installation

The Notebook requires `pandas`, `geopandas`, `geoplot` and `mapclassify` to run (and possibly other stuff too...)

You'll also need to install [NodeJS](https://nodejs.org/en/download/) and set up some notebook widgets if you want to render Kepler in your notebook. Full instructions for KeplerGL [are here](https://github.com/keplergl/kepler.gl/tree/master/bindings/kepler.gl-jupyter).

## Conda installation
```bash
# Conda

# Create environment
conda env create -f environment/environment.yml

# Activate environment
conda activate dsf-geo-presentation

# Install the Kernel
ipython kernel install --user --name=dsf-geo-presentation

# Run the notebook server
jupyter notebook
```

## Pip installation
```bash
# Create the environemnt
virtualenv dsf-geo-presentation

# Activate the environment (mac / linux)
source dsf-geo-presentation/bin/activate

# Activate the environment (windows)
dsf-geo-presentation\Scripts\activate

# Install dependencies
pip install -r environment/requirements.txt

# Install the Kernel
ipython kernel install --user --name=dsf-geo-presentation

# Run the notebook server
jupyter notebook
```

## Slides
The notebook is designed to be presented in slides mode. This can be activated as follows:
```bash
jupyter nbconvert *.ipynb --to slides --post serve
```


## Useful Links

General Resources:
* [What is GIS?](https://www.esri.com/en-us/what-is-gis/overview)
* [A Gentle Introduction to GIS](https://docs.qgis.org/3.4/en/docs/gentle_gis_introduction/index.html)
* [Coordinate Reference System (CRS) Finder](https://epsg.io/)
* [ONS Geography Hierarchies](https://www.ons.gov.uk/methodology/geography/ukgeographies/censusgeography)

Data Sources:
* [Data.gov.uk](https://data.gov.uk/)
* [ONS 2011 Census](https://www.ons.gov.uk/census/2011census)
* [Google Open Datasets (may require sign up to Google Cloud Platform)](https://console.cloud.google.com/marketplace/browse)
* [Data.world](https://data.world/)
* [Awesome Public Datasets (Github)](https://github.com/awesomedata/awesome-public-datasets)
* [Kaggle](https://www.kaggle.com/datasets)

Map Sources:
* [ONS Geoportal](http://geoportal.statistics.gov.uk/)
* [ESRI Data & Maps](https://www.arcgis.com/home/group.html?content=all&id=24838c2d95e14dd18c25e9bad55a7f82#overview)
* [DIVA GIS](http://www.diva-gis.org/gdata)

Supporting Data:
* [Source of data](https://data.gov.uk/dataset/cb7ae6f0-4be6-4935-9277-47e5ce24a11f/road-safety-data)
* [Supporting GCS Bucket](https://console.cloud.google.com/storage/browser/dsf-geo-presentation/)

Reference:
* [GeoPandas API Reference](https://geopandas.org/)
* [Mapshaper](https://mapshaper.org/)
* [Geoplot](https://residentmario.github.io/geoplot/index.html)
* [Mapclassify](https://github.com/pysal/mapclassify)
* [KeplerGL](https://kepler.gl/)
* [KeplerGL Github (Includes Installation Instructions)](https://github.com/keplergl/kepler.gl/tree/master/bindings/kepler.gl-jupyter)
* [KeplerGL User Guide](https://docs.kepler.gl/docs/keplergl-jupyter)
