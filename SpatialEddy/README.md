# SpatialEddy
 The SpatialEddy team focuses on spatializing flux tower data using NEON eddy-covariance data and environmental response functions. Our dataset includes geospatial flux maps and their respective quality masks. *This data is provided under a CC BY-SA 4.0 data license.*

 The Dataset includes:
 - 4 NEON sites: JORN, STEI, STER, TREE
 - Data covereage for 2019
 - carbon, H2O and heat flux at each site 


 ## Data Aquisition
 ---
 *SpatialEddy BenchFlux dataset is stored in a public GCP folder. No permissions are needed to grab the data, but make sure the Gcloud CLI correctly is installed https://cloud.google.com/sdk/docs/install*

 Make sure you authenticate first (follow the browser instructions after entering the command line below.)

`gcloud auth login`

CD into the local directory you plan to store the SpatialEddy data in.

`cd 'path/to/your/folder'`

Download the entire data bucket...

`gsutil -m cp -r gs://data-benchflux .`

or download at the site level - Treehaven for example.


`gsutil -m cp -r \
  "gs://data-benchflux/TREE" \
  .`

**warning** each site has an uncompressed size of ~8-10GB and a total dataset size of ~35.5GB, so this download will take some time to download.

## Getting Started
---
Visit tutorial.ipynb in the SpatialEddy/ directory to explore the SpatialEddy data.

To create a python environment for this tutorial, run

`pip install -r requirements.txt`

