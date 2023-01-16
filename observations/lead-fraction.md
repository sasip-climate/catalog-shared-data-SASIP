# satellite-derived lead fraction in the Arctic

The [repository](https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/observations/satellite/lead-fraction/catalog.html) contains files that contain:

- LF_corr: Lead fraction (in %) retrieved with the method of Rohrs et al (2012) with correction of the upper tie point suggested in Ivanova et al (2016). This value includes leads represented by open water and refrozen leads with thin ice. The valid range of values is 0-100%, while following values are masks:

```
105: where sea ice concentration is below 90 %
110: land
115: missing (or unrealistic) satellite data
```

- LF: Lead fraction (in %) retrieved with the method of Rohrs et al (2012). Same masks as for 1. are applied.

- Quality flag

 - missing (or unrealistic) satellite data
 - less certain values due to neighbouring satellite data missing

- SIC_ASI - sea ice concentration retrieved by the algorithm ASI (the product of the Bremen University)

- Latitude and longitude (-180 - +180)

All the variables are in polar stereographic projection with grid cell size (area in km2) provided in the file pixarea6km.mat, where nominal grid spacing is 6.25 km * 6.25 km (size of grid cells at the latitude of 70 N), dimensions: 1792*1216 grid cells.



Rohrs, J. and Kaleschke, L.: An algorithm to detect sea ice leads by using AMSR-E passive microwave imagery, The Cryosphere, 6, 343-352, doi:10.5194/tc-6-343-2012, 2012.

Rohrs, J., Kaleschke, L., Br?han, D., and Siligam, P. K.: Corrigendum to "An algorithm to detect sea ice leads by using AMSR-E passive microwave imagery" published in The Cryosphere, 6, 343?352, 2012, The Cryosphere, 6, 365-365, doi:10.5194/tc-6-365-2012, 2012.

Ivanova, N., Rampal, P., and Bouillon, S.: Error assessment of satellite-derived lead fraction in the Arctic, The Cryosphere, 10, 585-595, doi:10.5194/tc-10-585-2016, 2016.
