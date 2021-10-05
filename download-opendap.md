# How to download data from opendap

The adress is : https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/catalog.html
  - to download one file, click on it and then click on the HTTPServer link.
  - to download multiples files, use wget, for instance :
  
```
wget --no-check-certificate https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/fileServer/meomopendap/extract/NATL60-CJM165/1h/gridT/NATL60-CJM165_y20{12..13}m{01..12}d{01..31}.1h_gridT.nc
```
