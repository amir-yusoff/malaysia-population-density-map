# Creating Beautiful Population Density Maps with Python
## Mapping where the worlds 7.8 billion humans live with Python

### [Source Article](https://towardsdatascience.com/creating-beautiful-population-density-maps-with-python-fcdd84035e06)

---

### Data Preparation

There are a lot of population density datasets out there however for the purpose of this exercise we will use the [GHSL](https://ghsl.jrc.ec.europa.eu/download.php?ds=pop) — Global Human Settlement Layer. The data is freely available and terms of service can be found [here](chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/viewer.html?pdfurl=https%3A%2F%2Fghsl.jrc.ec.europa.eu%2Fdocuments%2FGHSL_Data_Package_2019.pdf%3Ft%3D1478q532234372&clen=4264054&chunk=true).
The first thing to do is to download the data to wherever you like to do your data visualisations. The data is available [here](https://ghsl.jrc.ec.europa.eu/download.php?ds=pop) and the specific file needed is the GHS population, 30 arcsec dataset from 2018. It is important to note that this tutorial will require the WGS84 projection. The data comes in the form of a tif file and can be read with rasterio.