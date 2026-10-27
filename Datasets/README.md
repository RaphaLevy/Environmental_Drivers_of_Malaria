All data used in the development of the paper will be separated according to their respective source:
- deter/ - Daily notified cases of deforestation in km² obtained from DETER ([TerraBrasilis - DETER (notices)](https://terrabrasilis.dpi.inpe.br/app/dashboard/alerts/biomes/amazonia-nb/daily/#)):
  - deter_deforestation_notification_data_2016_2024.csv: Daily deforestation data.
  - treated_deter_deforestation_data_2016_2024.csv: Aggregated daily deforestation data from 2016-01-01 to 2024-12-31. Missing dates from the original dataset were added with value 0 in all columns.
- mosqlimate_api/ - Contains two datasets of climate data obtained from the Mosqlimate datastore ([Mosqlimate API](https://api.mosqlimate.org/api/docs#/datastore/datastore_api_get_copernicus_brasil)):
  - climate_api_data_2016_2024.csv: Daily climatic data from 2016-01-01 to 2024-12-31, used for the main analysis
  - climate_api_data_aug_2003_jul_2004.csv: Daily climatic data from 2003-08-01 to 2004-07-31, used in the estimation of proper parameters of the birth rate, based on the work by de Barros, Honório and Arruda (2011)
- sivep/ - Daily cases of infection by malaria


The datasets may have undergone the following processing steps, as applicable:
- Data cleaning and consistency checks.
- Selection of observations within the study area and period.
- Temporal or spatial aggregation to obtain a common analytical resolution.
- Treatment of missing values and duplicate observations.
- Construction of derived variables used in the statistical analyses.

Data availability and reuse are subject to the terms and conditions of the original sources.

Datasets that are publicly available are referenced above. Data that cannot be redistributed are identified accordingly, together with instructions for obtaining them from their original providers, where permitted.

Please consult the original sources for applicable licensing and citation requirements.

