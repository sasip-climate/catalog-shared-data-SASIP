# Catalog of shared data between SASIP participants

Here you will find all the informations on the data that are shared among SASIP participants.
The datasets are physically stored on a SUMMER storage unit provided by UGA and paid by SASIP.

## What is available on the SUMMER storage

Here is a curated list of the data shared :

  - [Configuration files](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/configuration.md)
  - [Forcing datasets](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/forcings.md)
  - [Model outputs](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/outputs.md)
  - [Observation datasets](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/observations.md)

Some other datasets that are not stored on SUMMER but could be of interest for SASIP participants :

  - [Wave-in-ice Statistics from IS-2](https://doi.pangaea.de/10.1594/PANGAEA.918199)

## How to get access to the SUMMER storage

  - if you are working on Université Grenoble Alpes campus you can access it through a NFS mounting on your workstation, please send your IP address to data(at)sasip-climate.com to put you on the list
  - through your GRICAD account, more informations [here](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/gricad.md) 
  - for download only : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/catalog.html, more informations on how to download multiples files are [here](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/download-opendap.md)
  


## How to share a dataset on the SUMMER storage

  - put your data in a repository that has a meaningful name (ex ERAinterim-2012-2020-3h) in the right subdirectory (model-configuration, model-forcing, model-outputs, observations)
  - if needed, change the owner and rights to your directory so that everyone in the pr-sasip group can access it (like ```drwxrwxr-- 4 alberta pr-sasip```for instance)
  - provide a readme file that describes what, who, where, when the data was produced inside the repository (like [this one](https://github.com/sasip-climate/catalog-shared-data-SASIP/blob/main/forcings/ERAinterim-2012-2020-3h.md) for instance)
  - if you are the producer of the dataset, try as much as possible to follow the [FAIR principles](https://cloud.univ-grenoble-alpes.fr/index.php/apps/onlyoffice/s/p4BeQ8mfbniT9oM?fileId=354365064) that SASIP committed to endorse (rich metadata, doi, etc ...)
  - report the same informations on the catalog on github : create a md file in the right subdirectory of github (ex forcings/your-data.md) and make a link to it in forcings.md in this example
  - advertise that your data is available among SASIP participants using participants(at)sasip-climate.com mailing list !



    
    
