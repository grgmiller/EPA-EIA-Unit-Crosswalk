# EPA-EIA Unit Crosswalk
 Performs some cleaning of the crosswalk spreadsheet that matches @USEPA plant identifiers with @EIAgov plant identifiers

This code performs some cleaning on the EPA's EPA-EIA crosswalk spreadsheet using tables from https://github.com/catalyst-cooperative/pudl. 

This code performs the following transformations: 
1. renames all of the columns with all lowercase characters and underscores
2. matches all EPA ORIS_ID (`plant_id_epa`) with EIA ORISPL_ID (`plant_id_eia`). In the original crosswalk, most of these associations are missing. 
3. Applies the standard EIA fuel type code to the `fuel_type_primary` column
4. Imports primary fuel type data from EIA Form 860 based on the `plant_id_eia` and `generator_id`

In the future, I hope to match EIA `boiler_id` to the EPA `unit_id`, where missing. 

CSV Files included:
- `epa_eia_crosswalk_from_epa.csv` is a csv version of the excel file provided by the EPA. 
- `epa_eia_id_crosswalk.csv` is the output file from the ipython notebook

Crosswalk source: 
United States Environmental Protection Agency (EPA). “Power Sector Emissions Data: EPA-EIA Crosswalk.” Washington, DC: Office of Atmospheric Programs, Clean Air Markets Division.

PUDL Data Source: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3441606.svg)](https://doi.org/10.5281/zenodo.3441606)
