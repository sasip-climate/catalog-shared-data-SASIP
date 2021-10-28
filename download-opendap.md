# How to download data from opendap

The adress is : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/catalog.html
  - to download one file, click on it and then click on the HTTPServer link.
  - to download multiples files, use wget, for instance :
  
```
wget https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/fileServer/meomopendap/extract/SASIP/model-forcings/atmo_forcing/ERA5_Arctic/ERA5_v10_y{2011..2020}.nc
```

```
for var in u10 v10 t2m q2m d2m mtpr msr msl msdwlwrf; do wget https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/fileServer/meomopendap/extract/SASIP/model-forcings/atmo_forcing/ERA5_Arctic/ERA5_${var}_y{2011..2020}.nc; done
```

