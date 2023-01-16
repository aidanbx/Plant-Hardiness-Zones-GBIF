# Adding USDA Hardiness Zones to GBIF Occurence Data

This repository contains code for querying GBIF occurrence data for the United States and plotting it on a map of the US, with USDA Hardiness Zones represented as color.

Hardiness zones were gathered from the [Open Plant Hardiness Zones Repository](https://github.com/kgjenkins/ophz).


First, you will need to run the script to fetch the data from GBIF, then it will query the data against a GeoJSON file to match the occurrences with their respective temperature. Finally, it will plot the data on a map of the US using folium.

Here is an example of the final output:
<iframe src="map.html" width="100%" height="500"></iframe>

To run the code, simply execute the script in your preferred environment and the output will be the map.html file that you can open in your browser.

In case you would like to change the parameters or the GeoJSON file, make sure to edit the corresponding sections of the code.

Please note that the rate limit of the API should be considered, so you might want to use the pygbif library utility function gbif_key() to set your own key.

## Usage Instructions
---

1. Make sure you have the following dependencies installed:

    pygbif
    pandas
    numpy
    matplotlib
    geopandas
    folium

2. Clone the [Open Plant Hardiness Zones Repository](https://github.com/kgjenkins/ophz) into a folder named ophz

3. Enter the "# Plant-Hardiness-Zones-GBIF
