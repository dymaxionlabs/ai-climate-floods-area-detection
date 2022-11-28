# Susceptible flood area detection
## Description

Floods are one of the most often climate disasters in Honduras, mainly in Sula Valley. The informal settlement's population is particularly vulnerable due to the low-quality building construction.

The development of the susceptible flooded area model will contribute to information generation, which will allow good public policies.
As inputs, the model uses: (I) a raster dataset from optical satellites that represent conditioning factors (topographic and environmental) that can facilitate flood occurrence, (II)georeferenced information (ground truth) of flood past events.

DEM, slope, topographic wet index (TWI), land use and land cover (LULC), NDVI map, and distance to rivers and roads are the conditioning factors used in the input dataset.
The selection of these factors has depended on the area of interest characteristics and the availability of the data.  

## Requirements 

The tools **GDAL** y [Orfeo Toolbox](https://www.orfeo-toolbox.org/) are used in the first stage, the pre-processing of the data. In the following stages, our packages [satproc](https://github.com/dymaxionlabs/satproc) and [unetseg](https://github.com/dymaxionlabs/satproc) are used for dataset generation and for training and prediction process.

## Notebooks

This repository has a Jupyter Notebooks set, which describes the necessary steps:

1. [Training](notebooks/1_Entrenamiento.ipynb): Satellite imagery and ground truth are processed to generate the training dataset. Then, the model is trained and evaluated.
2. [Prediction](notebooks/2_Prediccion.ipynb): Prediction over the area of interest and prediction results processing.

## :handshake: Contributions

Bugs reports y *pull requests* could be done in the [issues page](https://github.com/dymaxionlabs/adefinir) of this repository. 

## :page_facing_up: License

The code is licensed under Apache 2.0. Refer to [LICENSE.txt](LICENSE.txt).
