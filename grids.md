# Grid examples for neXtSIM_DG

[This directory](https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/grids/catalog.html) contains several grid files that come from previous work with the old neXtSIM and NEMO, as well as some grids proposed for neXtSIM_DG. They are all netCDF files, but the content is subtly different, depending on the grid. Currently we have the following sub-directories and files:

 - [CREG](https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/grids/CREG/catalog.html) (regional North Atlantic-Arctic grid):
   - NEMO.nc
   - bathy_meter.nc
   - coordinates.nc

 - [NH_PS](https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/grids/NH_PS/catalog.html) (regional Arctic grid on a polar stereographic projection):
   - 12.5km_NH.nc
   - 25km_NH.nc
   - 3.125km_NH.nc
   - 6.25km_NH.nc

 - [SH_PS](https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/grids/SH_PS/catalog.html) (regional Antarctic grid on a polar stereographic projection):
   - 12.5km_SH_circle.nc
   - 25km_SH_circle.nc
   - 50km_SH_circle.nc
   - 6.25km_SH_circle.nc

 - [Split_ORCA2](https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/grids/Split_ORCA2/catalog.html) (global ORCA2 grid, split between northern and southern hemispheres):
   - NH_ORCA_R2_zps_domcfg.nc
   - SH_ORCA_R2_zps_domcfg.nc


These contain two types of files:

 - NEMO grid files (e.g. NH_ORCA_R2_zps_domcfg.nc, coordinates.nc). These contain geographic coordinates of the center, center of upper edge, center of right edge, and upper right corner for each grid cell (tracer, u, v, and f points). These are named glamt/gphit, glamu/gphiu, glamv/gphiv, glamf/glphif, respectively.
 - neXtSIM exchange grid files (e.g. NEMO.nc, 12.5km_NH.nc). These contain the geogrpahic coordinates of the center of the grid cell (plat, plon), as well as the geographic coordinates of all four corners of the grid (lat_corners, lon_corners). They also contain the cartesian coordinates of the coreners (x_corners, y_corners, z_corners), and the angle between the grid y axis and a vector pointing north (ptheta), taken at the grid center.
