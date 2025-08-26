# WW3

## Update 2025

Outputs from 2018 to 2022 : https://doi.org/10.11582/2025.ffmc0pcm
Associated paper available at : https://doi.org/10.1098/rsta.2021.0262


## Old version
Output of the WaveWatch3 model for the Arctic region at 25km resolution, 3-hourly snapshots, from Octobre 2018 to November 2019

Available on SUMMER at : `model-outputs/WW3-neXtSIM` or [directly on the opendap for download only](https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/SASIP/model-outputs/WW3-neXtSIM/catalog.html)

Data used for the study presented in "Modelling the Arctic wave-affected marginal ice zone, a comparison with ICESat-2 observations" (submitted to Phil. Trans. A) G. Boutin, T. Williams, C. Horvat and L. Brodeau

Content:

WW3NX025-012: Reference simulation (REF) of the publication "Modelling the Arctic wave-affected marginal ice zone, a comparison with ICESat-2 observations".

Contains WAVEWATCH III netCDF outputs with standard quantities (see WW3 manual for more details). Quantities used in the study are "hs" (significant wave height).

Also contains neXtSIM outputs. Quantities used in the study are "dmax" (maximum floe size), "dmean" (average floe size), "(siu,siv)" (sea ice drift u-v component (grid directions)). "sic" is sea ice concentration, "sit" sea ice thickness (cell averaged). Suffix "_young" is used to distinguish the "young ice category" from the total ice (see Appendix of Rampal et al. 2019, https://doi.org/10.5194/tc-13-2457-2019).

In the subfolder processed_WW3NX25-012 (and other simulations), you can find:

    - monthly neXtSIM model outputs (nxm.YYYYmMM.nc)
    - Hs monthly percentiles: ww3.YYYYmMM_hs_XXpercentile.nc (XX= value of percentile) computed for all cells with sea ice concentration >15% in 3h outputs
    - Hs monthly max values: ww3.YYYYmMM_hs_max_IceOnly.nc computed for all cells with sea ice concentration >15% in 3h outputs
    - neXtSIM quantities max values: nxm.YYYYmMM_dmax_max_IceOnly.nc (for dmax) computed for all cells with sea ice concentration >15% in 6h outputs
    - neXtSIM drift speed percentiles max values: nxm.YYYYmMM_sidrift_XXpercentile.nc (XX= value of percentile) computed for all cells with sea ice concentration >15% in 6h outputs

Experiments number correspondance with their names in the article: "WW3NX25-012":"REF" "WW3NX25-014":"DMG" "WW3NX25-010":"LOW BETAMAX" "WW3NX25-017":"NIDIS" "WW3NX25-015":"LFXST" "WW3NX25-016":"HBMX" "WW3NX25-020":"REF2"

(not here yet, cargo is bugging)
*contact Guillaume Boutin (at) nersc.no*

