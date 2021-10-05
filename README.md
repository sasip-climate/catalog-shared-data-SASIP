# Catalog of shared data between SASIP participants

Here you will find all the informations on the data that are shared among SASIP participants.
The datasets are physically stored on a SUMMER storage unit provided by UGA and paid by SASIP.

## How to get access to the SUMMER storage

  - if you are working on Université Grenoble Alpes campus, through a NFS mounting on your workstation, please send your IP address to data(at)sasip-climate.com to put you on the list
  - through your GRICAD account, create your account [here](https://perseus.univ-grenoble-alpes.fr/create-account/portal) and ask to be part of sasip group at data(at)sasip-climate.com, then when logged to dahu nodes you can access to storage at /summer/sasip 
  - for download only : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/catalog.html, more informations on how to download multiples files are [here]
  
## What is available on the SUMMER storage

Here is a curated list of the data shared :

  - [Configuration files](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/configuration.md)
  - [Forcing datasets](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/forcings.md)
  - [Model outputs](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/outputs.md)
  - [Observation datasets](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/observations.md)

## How to share a dataset on the SUMMER storage

  - put your data in a repository that has a meaningful name (ex ERAinterim-2012-2020-3h) in the right subdirectory (model-configuration, model-forcing, model-outputs, observations)
  - provide a readme file that describes what, who, where, when the data was produced inside the repository (like [this one](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/forcings/ERAinterim-2012-2020-3h.md) for instance)
  - if you are the producer of the dataset, try as much as possible to follow the [FAIR principles](https://docs.google.com/document/d/1moZo0tm6TOAgQRz365cTmpi2rT8mJePQvVMb5hlErsg/edit#heading=h.rw6dy5m1ru3m) that SASIP committed to endorse 
  - report the same informations on the catalog on github : create a md file in the right subdirectory of github (ex forcings/your-data.md) and make a link to it in forcings.md in this example
  - advertise that your data is available among SASIP participants using participants(at)sasip-climate.com mailing list



    
    
