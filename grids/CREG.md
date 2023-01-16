# regional North Atlantic-Arctic grid

This [directory](https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/grids/CREG/catalog.html) contains :

   - NEMO.nc : this file contains the geographic coordinates of the center of the grid cell (plat, plon), as well as the geographic coordinates of all four corners of the grid (lat_corners, lon_corners). It also contains the cartesian coordinates of the corners (x_corners, y_corners, z_corners), and the angle between the grid y axis and a vector pointing north (ptheta), taken at the grid center.

   - bathy_meter.nc
   - coordinates.nc

These contain geographic coordinates of the center, center of upper edge, center of right edge, and upper right corner for each grid cell (tracer, u, v, and f points). 
These are named glamt/gphit, glamu/gphiu, glamv/gphiv, glamf/glphif, respectively.
