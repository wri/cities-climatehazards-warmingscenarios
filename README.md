# Climate hazards for cities at 1.5C, 2C, and 3C of global warming

This repo contains code and data files necessary to replicate our estimates of 14 climate hazard indicators for 996 cities under 1.5C, 2C, and 3C of global warming above preindustrial baseline. Estimates are based on global climate models included in the [NEX-GDDP-CMIP6](https://www.nasa.gov/nasa-earth-exchange-nex/gddp/downscaled-climate-projections-nex-gddp-cmip6/) dataset. The methods underlying estimation of expected values of hazard magnitudes and of probabilities of threshold-magnitude exceedance are detailed in the WRI Technical Note [Wong and Switzer 2023](https://www.wri.org/research/estimating-future-local-climate-hazard-probabilities). The methodology defining the 14 climate hazards is forthcoming.

Models used in this analysis are given in this table.

| Model |	Institution |
|----------|----------|
| CanESM5	| Canadian Centre for Climate Modelling and Analysis |
| EC-Earth3-Veg-LR	| EC-Earth Consortium (Agencia Estatal de Meteorología, Spain; Barcelona Supercomputing Center, Spain; Consiglio Nazionale delle Ricerche–Instituto di Scienze dell'Atmosfera e del Clima, Italy; Danish Meteorological Institute, Denmark; Ente per le Nuove Technologie l'Energia e l'Ambiente, Italy; Finnish Meteorological Institute, Finland; Geomar, Germany; Irish Centre for High-End Computing, Ireland; International Centre for Theoretical Physics, Italy; Instituto Dom Luiz, Portugal; Institute for Marine and Atmospheric research Utrecht, Netherlands; Instituto Português do Mar e da Atmosfera, Portugal; Karlsruhe Institute of Technology, Germany; Royal Netherlands Meteorological Institute, Netherlands; Lund University, Sweden; Met Eireann, Ireland; Netherlands eScience Center, Netherlands; Norwegian University of Science and Technology, Norway; Oxford University, United Kingdom; SURFsara, Netherlands; Swedish Meteorological and Hydrological Institute, Sweden; Stockholm University, Sweden; Unite ASTR, Belgium; University College Dublin, Ireland; University of Bergen, Norway; University of Copenhagen, Denmark; University of Helsinki, Finland; University of Santiago de Compostela, Spain; Uppsala University, Sweden; Utrecht University, Netherlands; Vrije Universiteit Amsterdam, Netherlands; Wageningen University, Netherlands) |
| FGOALS-g3	| Chinese Academy of Sciences |
| GFDL-ESM4	| National Oceanic and Atmospheric Administration (United States), Geophysical Fluid Dynamics Laboratory |
| INM-CM5-0	| Institute for Numerical Mathematics, Russian Academy of Science |
| IPSL-CM6A-LR	|	Institut Pierre Simon Laplace |
| MIROC-ES2L	| Japan Agency for Marine-Earth Science and Technology |
| MRI-ESM2-0	| Meteorological Research Institute (Japan) |
| UKESM1-0-LL	| Met Office Hadley Centre; Natural Environment Research Council (United Kingdom); National Institute of Meteorological Sciences/Korea Meteorological Administration |


The files in this repo include
* **ghsl_500k**, which has the names and latlons of the 996 cities with metropolitan-area population greater than 500,000 according to the [GHSL Urban Centres Database](https://human-settlement.emergency.copernicus.eu/ghs_stat_ucdb2015mt_r2019a.php)
* **bmcf_[varname]** files, which include for each location the three best models (according to comparison with [ERA5](https://www.ecmwf.int/en/forecasts/dataset/ecmwf-reanalysis-v5) historical data) and calibration functions used to adjust modeled data to better fit the ERA5 data
* **scenarioyears_v2**, which includes the ten-year intervals we use to represent the warming levels for each of the nine climate models
*  **allrawdata_v2**, which are the outputs
* **calculate_climate_hazard_indicators_warming_scenarios_v1** a Jupyter notebook that generates all the estimates

Questions should be directed to Ted Wong at WRI (ted.wong@wri.org)
