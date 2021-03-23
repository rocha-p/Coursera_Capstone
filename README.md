#  CABA Clustering
### <center> By Pedro Ignacio Rocha </center>
-------

## Table of Contents

1. [Installation and Libraries](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation and Libraries  <a name="installation"></a>

Python version: `3.8.5`

You will need to install the following libraries:

* Pandas `import pandas as pd`
* Numpy `import numpy as np`
* Matplotlib - Pyplot `import matplotlib.pyplot as plt`
* Matplotlib - cm `import matplotlib.cm as cm`
* Matplotlib - colors `import matplotlib.colors as colors`
* Sklearn `from sklearn import preprocessing` `from sklearn.cluster import KMeans`
* Folium `import folium`
* Nominatim `from geopy.geocoders import Nominatim`
* json `import json`
* json_normalize `from pandas.io.json import json_normalize`
* request `import requests`

## Project Motivation<a name="motivation"></a>
This project analyzes the neighbourhoods in CABA to find the best ones to start a gastronomic business.

This project is of interest to people who plan to open a restaurant or people who already
have one and are thinking of opening a new branch. This project is also interesting for
people who plan to visit CABA to find out in which neighborhoods they can find a varied
gastronomic offer.

## File Descriptions <a name="files"></a>
Repository structure:
    
    clustering_caba_arg/                        # folder
    ├── README.md                               # read.md file 
    ├── Battle of Neighbourhoods Report.pdf     # report
    ├── Battle of Neighbourhoods.ipynb          # Jupyter notebook with the analysis
    ├── Ponderator_AVG_income.csv               # weighting used to adjust family income to each neighborhood
    ├── ingreso_por_comuna_familiar.csv         # Data set: average income per family per commune
    ├── oferta_gastronomica.csv                 # Data set: gastronomic offer in CABA
    ├── poblacion_por_barrio.csv                # Data set: CABA Neighbourhoods population

In this project I'll be using some Data Sets that you can find in the Buenos Aires Statistics Official Site:


[Gastronomic Offer in CABA](https://data.buenosaires.gob.ar/dataset/oferta-establecimientos-gastronomicos)

[Average total family income (ITF) according to commune. Buenos aires city. Years 2008/2019](https://www.estadisticaciudad.gob.ar/eyc/?p=82453)*

The Average total family income is calculated by commune so I calculated a weighting based on the price of the average M2 for sale in each neighborhood:
[Average price per m2 (dollars) of apartments for sale of 2 used rooms per neighborhood. Buenos aires city. 4th. 2006 / 4th quarter. quarter 2020](https://data.buenosaires.gob.ar/dataset/departamentos-venta/archivo/juqdkmgo-7031-resource)

Also I'll be using the *Foursquare API* to get the principal venues in each neighbourhood. You can check the documentation [HERE](https://developer.foursquare.com/docs)


## Licensing, Authors, Acknowledgements<a name="licensing"></a>
Licence: Atribucion 2.5 Argentina (CC BY 2.5 AR)
You can find the Licensing for the data and other descriptive information in the links above.
