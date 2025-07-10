SEA ICE OUTPUT FILES are at the 3-hourly frequency.
Variables available:


ncdump -h NANUK12-CPL00_3h_19961201_19961231_icemod.nc4
netcdf NANUK12-CPL00_3h_19961201_19961231_icemod {
dimensions:
   y = 1682 ;
   x = 1475 ;
   time_counter = UNLIMITED ; // (248 currently)
   axis_nbounds = 2 ;
variables:
   float nav_lat(y, x) ;
       nav_lat:standard_name = "latitude" ;
       nav_lat:long_name = "Latitude" ;
       nav_lat:units = "degrees_north" ;
   float nav_lon(y, x) ;
       nav_lon:standard_name = "longitude" ;
       nav_lon:long_name = "Longitude" ;
       nav_lon:units = "degrees_east" ;
   double time_instant(time_counter) ;
       time_instant:standard_name = "time" ;
       time_instant:long_name = "Time axis" ;
       time_instant:calendar = "gregorian" ;
       time_instant:units = "seconds since 1900-01-01 00:00:00" ;
       time_instant:time_origin = "1900-01-01 00:00:00" ;
       time_instant:bounds = "time_instant_bounds" ;
   double time_instant_bounds(time_counter, axis_nbounds) ;
   double time_counter(time_counter) ;
       time_counter:axis = "T" ;
       time_counter:standard_name = "time" ;
       time_counter:long_name = "Time axis" ;
       time_counter:calendar = "gregorian" ;
       time_counter:units = "seconds since 1900-01-01 00:00:00" ;
       time_counter:time_origin = "1900-01-01 00:00:00" ;
       time_counter:bounds = "time_counter_bounds" ;
   double time_counter_bounds(time_counter, axis_nbounds) ;
   float siconc-t(time_counter, y, x) ;
       siconc-t:standard_name = "sea_ice_area_fraction" ;
       siconc-t:long_name = "Sea-ice area fraction" ;
       siconc-t:units = "" ;
       siconc-t:online_operation = "instant" ;
       siconc-t:interval_operation = "300 s" ;
       siconc-t:interval_write = "3 h" ;
       siconc-t:cell_methods = "time: point (interval: 300 s)" ;
       siconc-t:_FillValue = 1.e+20f ;
       siconc-t:missing_value = 1.e+20f ;
       siconc-t:coordinates = "time_instant nav_lat nav_lon" ;
   float sivolu(time_counter, y, x) ;
       sivolu:standard_name = "sea_ice_volume" ;
       sivolu:long_name = "Sea-ice volume per area" ;
       sivolu:units = "m" ;
       sivolu:valid_min = 0. ;
       sivolu:valid_max = 5. ;
       sivolu:online_operation = "instant" ;
       sivolu:interval_operation = "300 s" ;
       sivolu:interval_write = "3 h" ;
       sivolu:cell_methods = "time: point (interval: 300 s)" ;
       sivolu:_FillValue = 1.e+20f ;
       sivolu:missing_value = 1.e+20f ;
       sivolu:coordinates = "time_instant nav_lat nav_lon" ;
   float snvolu(time_counter, y, x) ;
       snvolu:standard_name = "snow_volume" ;
       snvolu:long_name = "Snow volume per area" ;
       snvolu:units = "m" ;
       snvolu:valid_min = 0. ;
       snvolu:valid_max = 3. ;
       snvolu:online_operation = "instant" ;
       snvolu:interval_operation = "300 s" ;
       snvolu:interval_write = "3 h" ;
       snvolu:cell_methods = "time: point (interval: 300 s)" ;
       snvolu:_FillValue = 1.e+20f ;
       snvolu:missing_value = 1.e+20f ;
       snvolu:coordinates = "time_instant nav_lat nav_lon" ;
   float damage-t(time_counter, y, x) ;
       damage-t:standard_name = "sea_ice_damage_t" ;
       damage-t:long_name = "ice damage at T-points" ;
       damage-t:units = "" ;
       damage-t:online_operation = "instant" ;
       damage-t:interval_operation = "300 s" ;
       damage-t:interval_write = "3 h" ;
       damage-t:cell_methods = "time: point (interval: 300 s)" ;
       damage-t:_FillValue = 1.e+20f ;
       damage-t:missing_value = 1.e+20f ;
       damage-t:coordinates = "time_instant nav_lat nav_lon" ;
   float siconc-f(time_counter, y, x) ;
       siconc-f:standard_name = "sea_ice_area_fraction_f" ;
       siconc-f:long_name = "Sea-ice area fraction @F" ;
       siconc-f:units = "" ;
       siconc-f:online_operation = "instant" ;
       siconc-f:interval_operation = "300 s" ;
       siconc-f:interval_write = "3 h" ;
       siconc-f:cell_methods = "time: point (interval: 300 s)" ;
       siconc-f:_FillValue = 1.e+20f ;
       siconc-f:missing_value = 1.e+20f ;
       siconc-f:coordinates = "time_instant nav_lat nav_lon" ;
   float sithic-f(time_counter, y, x) ;
       sithic-f:standard_name = "sea_ice_thickness_f" ;
       sithic-f:long_name = "Sea-ice thickness @F" ;
       sithic-f:units = "m" ;
       sithic-f:valid_min = 0. ;
       sithic-f:valid_max = 5. ;
       sithic-f:online_operation = "instant" ;
       sithic-f:interval_operation = "300 s" ;
       sithic-f:interval_write = "3 h" ;
       sithic-f:cell_methods = "time: point (interval: 300 s)" ;
       sithic-f:_FillValue = 1.e+20f ;
       sithic-f:missing_value = 1.e+20f ;
       sithic-f:coordinates = "time_instant nav_lat nav_lon" ;
   float damage-f(time_counter, y, x) ;
       damage-f:standard_name = "sea_ice_damage_f" ;
       damage-f:long_name = "ice damage at F-points" ;
       damage-f:units = "" ;
       damage-f:online_operation = "instant" ;
       damage-f:interval_operation = "300 s" ;
       damage-f:interval_write = "3 h" ;
       damage-f:cell_methods = "time: point (interval: 300 s)" ;
       damage-f:_FillValue = 1.e+20f ;
       damage-f:missing_value = 1.e+20f ;
       damage-f:coordinates = "time_instant nav_lat nav_lon" ;
   float sidive-t(time_counter, y, x) ;
       sidive-t:standard_name = "divergence_of_sea_ice_velocity_t" ;
       sidive-t:long_name = "Divergence of the sea-ice velocity field @T" ;
       sidive-t:units = "s-1" ;
       sidive-t:valid_min = -5.e-06 ;
       sidive-t:valid_max = 5.e-06 ;
       sidive-t:online_operation = "instant" ;
       sidive-t:interval_operation = "300 s" ;
       sidive-t:interval_write = "3 h" ;
       sidive-t:cell_methods = "time: point (interval: 300 s)" ;
       sidive-t:_FillValue = 1.e+20f ;
       sidive-t:missing_value = 1.e+20f ;
       sidive-t:coordinates = "time_instant nav_lat nav_lon" ;
   float sishear-f(time_counter, y, x) ;
       sishear-f:standard_name = "shear_rate_of_sea_ice_velocity_f" ;
       sishear-f:long_name = "Strain shear rate of sea-ice velocity field @F" ;
       sishear-f:units = "s-1" ;
       sishear-f:valid_min = -5.e-06 ;
       sishear-f:valid_max = 5.e-06 ;
       sishear-f:online_operation = "instant" ;
       sishear-f:interval_operation = "300 s" ;
       sishear-f:interval_write = "3 h" ;
       sishear-f:cell_methods = "time: point (interval: 300 s)" ;
       sishear-f:_FillValue = 1.e+20f ;
       sishear-f:missing_value = 1.e+20f ;
       sishear-f:coordinates = "time_instant nav_lat nav_lon" ;
   float sidefo-t(time_counter, y, x) ;
       sidefo-t:standard_name = "deformation_rate_of_sea_ice_velocity_t" ;
       sidefo-t:long_name = "Deformation rate of sea-ice velocity field @T" ;
       sidefo-t:units = "s-1" ;
       sidefo-t:valid_min = 0. ;
       sidefo-t:valid_max = 1.e-05 ;
       sidefo-t:online_operation = "instant" ;
       sidefo-t:interval_operation = "300 s" ;
       sidefo-t:interval_write = "3 h" ;
       sidefo-t:cell_methods = "time: point (interval: 300 s)" ;
       sidefo-t:_FillValue = 1.e+20f ;
       sidefo-t:missing_value = 1.e+20f ;
       sidefo-t:coordinates = "time_instant nav_lat nav_lon" ;
   float sivort-f(time_counter, y, x) ;
       sivort-f:standard_name = "vorticity_of_sea_ice_velocity_f" ;
       sivort-f:long_name = "Vorticity of sea-ice velocity field @F" ;
       sivort-f:units = "s-1" ;
       sivort-f:valid_min = -1.e-05 ;
       sivort-f:valid_max = 1.e-05 ;
       sivort-f:online_operation = "instant" ;
       sivort-f:interval_operation = "300 s" ;
       sivort-f:interval_write = "3 h" ;
       sivort-f:cell_methods = "time: point (interval: 300 s)" ;
       sivort-f:_FillValue = 1.e+20f ;
       sivort-f:missing_value = 1.e+20f ;
       sivort-f:coordinates = "time_instant nav_lat nav_lon" ;
   float simxshr-t(time_counter, y, x) ;
       simxshr-t:standard_name = "maximum_shear_of_sea_ice_velocity_t" ;
       simxshr-t:long_name = "Maximum shear of sea-ice velocity field @T" ;
       simxshr-t:units = "s-1" ;
       simxshr-t:valid_min = 0. ;
       simxshr-t:valid_max = 1.e-05 ;
       simxshr-t:online_operation = "instant" ;
       simxshr-t:interval_operation = "300 s" ;
       simxshr-t:interval_write = "3 h" ;
       simxshr-t:cell_methods = "time: point (interval: 300 s)" ;
       simxshr-t:_FillValue = 1.e+20f ;
       simxshr-t:missing_value = 1.e+20f ;
       simxshr-t:coordinates = "time_instant nav_lat nav_lon" ;
   float u_ice-u(time_counter, y, x) ;
       u_ice-u:standard_name = "sea_ice_x_velocity" ;
       u_ice-u:long_name = "X-component of sea ice velocity @U" ;
       u_ice-u:units = "m/s" ;
       u_ice-u:valid_min = -0.5 ;
       u_ice-u:valid_max = 0.5 ;
       u_ice-u:online_operation = "instant" ;
       u_ice-u:interval_operation = "300 s" ;
       u_ice-u:interval_write = "3 h" ;
       u_ice-u:cell_methods = "time: point (interval: 300 s)" ;
       u_ice-u:_FillValue = 1.e+20f ;
       u_ice-u:missing_value = 1.e+20f ;
       u_ice-u:coordinates = "time_instant nav_lat nav_lon" ;
   float v_ice-v(time_counter, y, x) ;
       v_ice-v:standard_name = "sea_ice_y_velocity" ;
       v_ice-v:long_name = "Y-component of sea ice velocity @V" ;
       v_ice-v:units = "m/s" ;
       v_ice-v:valid_min = -0.5 ;
       v_ice-v:valid_max = 0.5 ;
       v_ice-v:online_operation = "instant" ;
       v_ice-v:interval_operation = "300 s" ;
       v_ice-v:interval_write = "3 h" ;
       v_ice-v:cell_methods = "time: point (interval: 300 s)" ;
       v_ice-v:_FillValue = 1.e+20f ;
       v_ice-v:missing_value = 1.e+20f ;
       v_ice-v:coordinates = "time_instant nav_lat nav_lon" ;
   float ice_sigI-t(time_counter, y, x) ;
       ice_sigI-t:standard_name = "normal_stress_invariant_t" ;
       ice_sigI-t:long_name = "Normal stress aka 1st invariant of stress tensor @T" ;
       ice_sigI-t:units = "Pa" ;
       ice_sigI-t:valid_min = -50000. ;
       ice_sigI-t:valid_max = 5000. ;
       ice_sigI-t:online_operation = "instant" ;
       ice_sigI-t:interval_operation = "300 s" ;
       ice_sigI-t:interval_write = "3 h" ;
       ice_sigI-t:cell_methods = "time: point (interval: 300 s)" ;
       ice_sigI-t:_FillValue = 1.e+20f ;
       ice_sigI-t:missing_value = 1.e+20f ;
       ice_sigI-t:coordinates = "time_instant nav_lat nav_lon" ;
   float ice_sigII-t(time_counter, y, x) ;
       ice_sigII-t:standard_name = "shear_stress_invariant_t" ;
       ice_sigII-t:long_name = "Shear stress aka 2nd invariant of stress tensor @T" ;
       ice_sigII-t:units = "Pa" ;
       ice_sigII-t:valid_min = 0. ;
       ice_sigII-t:valid_max = 30000. ;
       ice_sigII-t:online_operation = "instant" ;
       ice_sigII-t:interval_operation = "300 s" ;
       ice_sigII-t:interval_write = "3 h" ;
       ice_sigII-t:cell_methods = "time: point (interval: 300 s)" ;
       ice_sigII-t:_FillValue = 1.e+20f ;
       ice_sigII-t:missing_value = 1.e+20f ;
       ice_sigII-t:coordinates = "time_instant nav_lat nav_lon" ;









OCEAN variables are daily averages


netcdf NANUK12-CPL00_1d_19971101_19971130_gridT {
dimensions:
   y = 1682 ;
   x = 1475 ;
   deptht = 31 ;
   axis_nbounds = 2 ;
   time_counter = UNLIMITED ; // (30 currently)
variables:
   float nav_lat(y, x) ;
       nav_lat:standard_name = "latitude" ;
       nav_lat:long_name = "Latitude" ;
       nav_lat:units = "degrees_north" ;
   float nav_lon(y, x) ;
       nav_lon:standard_name = "longitude" ;
       nav_lon:long_name = "Longitude" ;
       nav_lon:units = "degrees_east" ;
   float deptht(deptht) ;
       deptht:name = "deptht" ;
       deptht:long_name = "Vertical T levels" ;
       deptht:units = "m" ;
       deptht:positive = "down" ;
       deptht:bounds = "deptht_bounds" ;
   float deptht_bounds(deptht, axis_nbounds) ;
       deptht_bounds:units = "m" ;
   double time_centered(time_counter) ;
       time_centered:standard_name = "time" ;
       time_centered:long_name = "Time axis" ;
       time_centered:calendar = "gregorian" ;
       time_centered:units = "seconds since 1900-01-01 00:00:00" ;
       time_centered:time_origin = "1900-01-01 00:00:00" ;
       time_centered:bounds = "time_centered_bounds" ;
   double time_centered_bounds(time_counter, axis_nbounds) ;
   double time_counter(time_counter) ;
       time_counter:axis = "T" ;
       time_counter:standard_name = "time" ;
       time_counter:long_name = "Time axis" ;
       time_counter:calendar = "gregorian" ;
       time_counter:units = "seconds since 1900-01-01 00:00:00" ;
       time_counter:time_origin = "1900-01-01 00:00:00" ;
       time_counter:bounds = "time_counter_bounds" ;
   double time_counter_bounds(time_counter, axis_nbounds) ;
   float votemper(time_counter, deptht, y, x) ;
       votemper:standard_name = "sea_water_potential_temperature" ;
       votemper:long_name = "temperature" ;
       votemper:units = "degC" ;
       votemper:online_operation = "average" ;
       votemper:interval_operation = "300 s" ;
       votemper:interval_write = "1 d" ;
       votemper:cell_methods = "time: mean (interval: 300 s)" ;
       votemper:_FillValue = 1.e+20f ;
       votemper:missing_value = 1.e+20f ;
       votemper:coordinates = "time_centered nav_lat nav_lon" ;
   float vosaline(time_counter, deptht, y, x) ;
       vosaline:standard_name = "sea_water_practical_salinity" ;
       vosaline:long_name = "salinity" ;
       vosaline:units = "1e-3" ;
       vosaline:online_operation = "average" ;
       vosaline:interval_operation = "300 s" ;
       vosaline:interval_write = "1 d" ;
       vosaline:cell_methods = "time: mean (interval: 300 s)" ;
       vosaline:_FillValue = 1.e+20f ;
       vosaline:missing_value = 1.e+20f ;
       vosaline:coordinates = "time_centered nav_lat nav_lon" ;
   float tos(time_counter, y, x) ;
       tos:standard_name = "bulk_sea_surface_temperature" ;
       tos:long_name = "Bulk sea surface temperature" ;
       tos:units = "degC" ;
       tos:online_operation = "average" ;
       tos:interval_operation = "300 s" ;
       tos:interval_write = "1 d" ;
       tos:cell_methods = "time: mean (interval: 300 s)" ;
       tos:_FillValue = 1.e+20f ;
       tos:missing_value = 1.e+20f ;
       tos:coordinates = "time_centered nav_lat nav_lon" ;
   float sos(time_counter, y, x) ;
       sos:standard_name = "sea_surface_salinity" ;
       sos:long_name = "sea surface salinity" ;
       sos:units = "1e-3" ;
       sos:online_operation = "average" ;
       sos:interval_operation = "300 s" ;
       sos:interval_write = "1 d" ;
       sos:cell_methods = "time: mean (interval: 300 s)" ;
       sos:_FillValue = 1.e+20f ;
       sos:missing_value = 1.e+20f ;
       sos:coordinates = "time_centered nav_lat nav_lon" ;
   float zos(time_counter, y, x) ;
       zos:standard_name = "sea_surface_height_above_geoid" ;
       zos:long_name = "sea surface height" ;
       zos:units = "m" ;
       zos:online_operation = "average" ;
       zos:interval_operation = "300 s" ;
       zos:interval_write = "1 d" ;
       zos:cell_methods = "time: mean (interval: 300 s)" ;
       zos:_FillValue = 1.e+20f ;
       zos:missing_value = 1.e+20f ;
       zos:coordinates = "time_centered nav_lat nav_lon" ;
   float sowaflup(time_counter, y, x) ;
       sowaflup:standard_name = "water_flux_out_of_sea_ice_and_sea_water" ;
       sowaflup:long_name = "Net Upward Water Flux" ;
       sowaflup:units = "kg/m2/s" ;
       sowaflup:online_operation = "average" ;
       sowaflup:interval_operation = "300 s" ;
       sowaflup:interval_write = "1 d" ;
       sowaflup:cell_methods = "time: mean (interval: 300 s)" ;
       sowaflup:_FillValue = 1.e+20f ;
       sowaflup:missing_value = 1.e+20f ;
       sowaflup:coordinates = "time_centered nav_lat nav_lon" ;
   float runoffs(time_counter, y, x) ;
       runoffs:standard_name = "water_flux_into_sea_water_from_rivers" ;
       runoffs:long_name = "River Runoffs" ;
       runoffs:units = "kg/m2/s" ;
       runoffs:online_operation = "average" ;
       runoffs:interval_operation = "300 s" ;
       runoffs:interval_write = "1 d" ;
       runoffs:cell_methods = "time: mean (interval: 300 s)" ;
       runoffs:_FillValue = 1.e+20f ;
       runoffs:missing_value = 1.e+20f ;
       runoffs:coordinates = "time_centered nav_lat nav_lon" ;
   float soshfldo(time_counter, y, x) ;
       soshfldo:standard_name = "net_downward_shortwave_flux_at_sea_water_surface" ;
       soshfldo:long_name = "Shortwave Radiation" ;
       soshfldo:units = "W/m2" ;
       soshfldo:online_operation = "average" ;
       soshfldo:interval_operation = "300 s" ;
       soshfldo:interval_write = "1 d" ;
       soshfldo:cell_methods = "time: mean (interval: 300 s)" ;
       soshfldo:_FillValue = 1.e+20f ;
       soshfldo:missing_value = 1.e+20f ;
       soshfldo:coordinates = "time_centered nav_lat nav_lon" ;
   float sosfldow(time_counter, y, x) ;
       sosfldow:long_name = "Downward salt flux" ;
       sosfldow:units = "g/m2/s" ;
       sosfldow:online_operation = "average" ;
       sosfldow:interval_operation = "300 s" ;
       sosfldow:interval_write = "1 d" ;
       sosfldow:cell_methods = "time: mean (interval: 300 s)" ;
       sosfldow:_FillValue = 1.e+20f ;
       sosfldow:missing_value = 1.e+20f ;
       sosfldow:coordinates = "time_centered nav_lat nav_lon" ;
   float sohefldo(time_counter, y, x) ;
       sohefldo:standard_name = "surface_downward_heat_flux_in_sea_water" ;
       sohefldo:long_name = "Net Downward Heat Flux" ;
       sohefldo:units = "W/m2" ;
       sohefldo:online_operation = "average" ;
       sohefldo:interval_operation = "300 s" ;
       sohefldo:interval_write = "1 d" ;
       sohefldo:cell_methods = "time: mean (interval: 300 s)" ;
       sohefldo:_FillValue = 1.e+20f ;
       sohefldo:missing_value = 1.e+20f ;
       sohefldo:coordinates = "time_centered nav_lat nav_lon" ;
   float somxl010(time_counter, y, x) ;
       somxl010:standard_name = "ocean_mixed_layer_thickness_defined_by_sigma_theta" ;
       somxl010:long_name = "Mixed Layer Depth (dsigma = 0.01 wrt 10m)" ;
       somxl010:units = "m" ;
       somxl010:online_operation = "average" ;
       somxl010:interval_operation = "300 s" ;
       somxl010:interval_write = "1 d" ;
       somxl010:cell_methods = "time: mean (interval: 300 s)" ;
       somxl010:_FillValue = 1.e+20f ;
       somxl010:missing_value = 1.e+20f ;
       somxl010:coordinates = "time_centered nav_lat nav_lon" ;
   float somixhgt(time_counter, y, x) ;
       somixhgt:standard_name = "ocean_mixed_layer_thickness_defined_by_vertical_tracer_diffusivity" ;
       somixhgt:long_name = "Turbocline depth (Kz = 5e-4)" ;
       somixhgt:units = "m" ;
       somixhgt:online_operation = "average" ;
       somixhgt:interval_operation = "300 s" ;
       somixhgt:interval_write = "1 d" ;
       somixhgt:cell_methods = "time: mean (interval: 300 s)" ;
       somixhgt:_FillValue = 1.e+20f ;
       somixhgt:missing_value = 1.e+20f ;
       somixhgt:coordinates = "time_centered nav_lat nav_lon" ;
   float taum(time_counter, y, x) ;
       taum:standard_name = "magnitude_of_surface_downward_stress" ;
       taum:long_name = "wind stress module" ;
       taum:units = "N/m2" ;
       taum:online_operation = "average" ;
       taum:interval_operation = "300 s" ;
       taum:interval_write = "1 d" ;
       taum:cell_methods = "time: mean (interval: 300 s)" ;
       taum:_FillValue = 1.e+20f ;
       taum:missing_value = 1.e+20f ;
       taum:coordinates = "time_centered nav_lat nav_lon" ;
   float ice_cover(time_counter, y, x) ;
       ice_cover:standard_name = "sea_ice_area_fraction" ;
       ice_cover:long_name = "Ice fraction" ;
       ice_cover:units = "1" ;
       ice_cover:online_operation = "average" ;
       ice_cover:interval_operation = "300 s" ;
       ice_cover:interval_write = "1 d" ;
       ice_cover:cell_methods = "time: mean (interval: 300 s)" ;
       ice_cover:_FillValue = 1.e+20f ;
       ice_cover:missing_value = 1.e+20f ;
       ice_cover:coordinates = "time_centered nav_lat nav_lon" ;

MASK AND GRID FILE

netcdf mesh_mask_NANUK12_L31_4.2 {
dimensions:
	x = 1475 ;
	y = 1682 ;
	nav_lev = 31 ;
	time_counter = UNLIMITED ; // (1 currently)
variables:
	float nav_lon(y, x) ;
	float nav_lat(y, x) ;
	float nav_lev(nav_lev) ;
	float time_counter(time_counter) ;
	byte tmask(time_counter, nav_lev, y, x) ;
 "sea-land mask for T-grid"
	byte umask(time_counter, nav_lev, y, x) ;
  "sea-land mask for U-grid"
	byte vmask(time_counter, nav_lev, y, x) ;
  "sea-land mask for V-grid"
	byte fmask(time_counter, nav_lev, y, x) ;
  "sea-land mask for F-grid"
	byte tmaskutil(time_counter, y, x) ;
  "surface sea-land mask for T-grid"
	byte umaskutil(time_counter, y, x) ;
  "surface sea-land mask for U-grid"
	byte vmaskutil(time_counter, y, x) ;
  "surface sea-land mask for V-grid"
	double glamt(time_counter, y, x) ;
  "geographic longitude for T-grid"
	double glamu(time_counter, y, x) ;
  "geographic longitude for U-grid"
	double glamv(time_counter, y, x) ;
  "geographic longitude for V-grid"
	double glamf(time_counter, y, x) ;
  "geographic longitude for F-grid"
	double gphit(time_counter, y, x) ;
  "geographic latitude for T-grid"
	double gphiu(time_counter, y, x) ;
  "geographic latitude for T-grid"
	double gphiv(time_counter, y, x) ;
  "geographic latitude for T-grid"
	double gphif(time_counter, y, x) 
  "geographic latitude for T-grid"
	double e1t(time_counter, y, x) ;
  "zonal scale factor for T-grid"
	double e1u(time_counter, y, x) ;
  "zonal scale factor for U-grid"
	double e1v(time_counter, y, x) ;
  "zonal scale factor for V-grid"
	double e1f(time_counter, y, x) ;
  "zonal scale factor for F-grid"
	double e2t(time_counter, y, x) ;
  "meridional scale factor for T-grid"
	double e2u(time_counter, y, x) ;
  "meridional scale factor for U-grid"
	double e2v(time_counter, y, x) ;
  "meridional scale factor for V-grid"
	double e2f(time_counter, y, x) ;
  "meridional scale factor for F-grid"
	double ff_f(time_counter, y, x) ;
  "Coriolis parameter for grid-F" 
	double ff_t(time_counter, y, x) ;
  "Coriolis parameter for grid-T" 
	int mbathy(time_counter, y, x) ;
	int misf(time_counter, y, x) ;
	double e3t_1d(time_counter, nav_lev) ;
	double e3w_1d(time_counter, nav_lev) ;
	double e3t_0(time_counter, nav_lev, y, x) ;
	double e3u_0(time_counter, nav_lev, y, x) ;
	double e3v_0(time_counter, nav_lev, y, x) ;
	double e3f_0(time_counter, nav_lev, y, x) ;
	double e3w_0(time_counter, nav_lev, y, x) ;
	double e3uw_0(time_counter, nav_lev, y, x) ;
	double e3vw_0(time_counter, nav_lev, y, x) ;
	double gdept_1d(time_counter, nav_lev) ;
	double gdepw_1d(time_counter, nav_lev) ;
	double gdept_0(time_counter, nav_lev, y, x) ;
	double gdepw_0(time_counter, nav_lev, y, x) ;

