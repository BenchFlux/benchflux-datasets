# CarbonSense

The CarbonSense team focuses on aggregating multimodal datasets for deep learning models in carbon flux modelling. Our dataset includes:

- Eddy covariance observations from AmeriFlux, ICOS, and FLUXNET
- MODIS satellite imagery
- Phenocam imagery from available sites

The supplied data subset does not have the phenocam imagery as this would balloon the site from 20GB to 150GB, and is not relevant for Benchflux at this time.

## Data acquisition

To download and extract the data (requires access to the Benchflux project via gcloud):

`gcloud storage cp gs://benchflux-team-data/carbonsense_v2_no_phenocam.tar.gz .`

Once the download is complete, the data can be extracted with:

`tar xzvf carbonsense_v2_no_phenocam.tar.gz`

This tarball has a compressed size of ~6 GB and an uncompressed size of ~20 GB

## Getting Started

After extracting the data, run the tutorial.ipynb notebook located in the carbonsense/ directory to begin exploring the dataset. Our tutorial uses a minimal set of Python libraries such as pandas, numpy, and matplotlib, so we chose not to include a requirements.txt file as this should work with almost any recent Python version.