# EPA-EIA Unit Crosswalk
 Performs some cleaning of the EPA's crosswalk spreadsheet

This code performs some cleaning on the EPA's EPA-EIA crosswalk spreadsheet using tables from https://github.com/catalyst-cooperative/pudl. 

At this point, this package simply matches all EPA ORIS_ID (`plant_id_epa`) with EIA ORISPL_ID (`plant_id_eia`). In the future, I hope to standardize unit fuel type codes and help match EIA boiler_id to the EPA unit_id, where missing. 

epa_eia_crosswalk_from_epa.csv is a csv version of the excel file provided by the EPA. 
epa_eia_id_crosswalk.csv is the output file from the ipython notebook

Crosswalk source: 
United States Environmental Protection Agency (EPA). “Power Sector Emissions Data: EPA-EIA Crosswalk.” Washington, DC: Office of Atmospheric Programs, Clean Air Markets Division.

PUDL Data Source: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3441606.svg)](https://doi.org/10.5281/zenodo.3441606)
