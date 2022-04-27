# Small Arctic at 10km resolution

For year 2006 : from February, 1st to December, 28th 

Available on SUMMER at : `model-configurations/nextsim/small_arctic_10km` or directly on the [opendap](https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/model-configurations/nextsim/small_arctic_10km/catalog.html) for download only

You can find in :
   - scripts :
      - the namelist : bbm_control.cfg
      - the initial mesh file : small_arctic_10km.msh
      - the run script : small_arctic_10km.msh (adapt the paths to your architecture)
      - the mpp files for stereographic projections (taken from nextsim github repo) : NpsNextsim.mpp and NpsASR.mpp
   - files :
      - the arctic topography ETOPO : ETOPO_Arctic_2arcmin.nc
      - atmospheric forcing files : ERA5*
      - oceanic forcing files : TP4*
      - PIOMAS ?

Contact : Einar.Olason[at]nersc.no
