# SpatialEddy
 The SpatialEddy team 



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



