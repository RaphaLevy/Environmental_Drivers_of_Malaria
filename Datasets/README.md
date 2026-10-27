All data used in the development of the paper will be separated according to their respective source:
- deter/ - Daily notified cases of deforestation in km² obtained from DETER ([TerraBrasilis - DETER (notices)](https://terrabrasilis.dpi.inpe.br/app/dashboard/alerts/biomes/amazonia-nb/daily/#)):
  - deter_deforestation_notification_data_2016_2024.csv: Daily deforestation data.
  - treated_deter_deforestation_data_2016_2024.csv: Aggregated daily deforestation data from 2016-01-01 to 2024-12-31. Missing dates from the original dataset were added with value 0 in all columns.
- ibge/ - Contains two datasets of population data obtained from IBGE:
  - ibge_manaus_fixed_rural_population_data_2016_2024.csv: Contains estimated daily rural and total population of Manaus
  - ibge_manaus_population_data_2016_2024.csv: Contains interpolated daily population data of Manaus
    - 2000: [IBGE 2000](https://biblioteca.ibge.gov.br/index.php/biblioteca-catalogo?view=detalhes&id=7308)
    - 2010: [IBGE 2010](https://www.ibge.gov.br/estatisticas/sociais/populacao/9662-censo-demografico-2010.html?=&t=resultados)
    - 2022: [IBGE 2022](https://cidades.ibge.gov.br/brasil/am/manaus/panorama)
    - 2025: [IBGE 2025](https://www.ibge.gov.br/cidades-e-estados/am/manaus.html)
- inpe/ - Contains a single dataset of daily fire counts data gathered by INPE, obtained from the Base dos Dados dataset, from 2016-01-01 to 2024-12-31
([Banco de Dados de Queimadas](https://basedosdados.org/dataset/f06f3cdc-b539-409b-b311-1ff8878fb8d9?table=a3696dc2-4dd1-4f7e-9769-6aa16a1556b8))
- mapbiomas/ - Contains a single dataset of monthly tendencies of burnt out areas in hectares, from 2017-01 to 2023-12, obtained from MapBiomas ([Mapbiomas - Monthly trends by year](https://plataforma.brasil.mapbiomas.org/fogo-copia-1h7mac/fogo-copia-1h7mac_monthly-433exq?activeBaseMap=1&layersOpacity=100&activeModule=fire&activeModuleContent=fire:fire_monthly&activeYear=2023&mapPosition=-2.573422,-59.981338,9&timelineLimitsRange=1985,2023&baseParams[territoryType]=4&baseParams[territory]=146&baseParams[territories]=146;1302603%20-%20Manaus%20(AM);4;Munic%C3%ADpio;-3.22220882399995;-60.802727218;-1.92430443799998;-59.1599483219999&baseParams[activeClassTreeOptionValue]=fire_monthly&baseParams[activeClassTreeNodeIds]=603,604,605,606,607,608,609,610,611,612,613,614&baseParams[activeSubmodule]=fire_monthly&baseParams[yearRange]=1985-2023&tl[id]=66&tl[themeKey]=fogo-copia-1h7mac&tl[subthemeKey]=fogo-copia-1h7mac_monthly-433exq&tl[pixelValues][]=1&tl[pixelValues][]=2&tl[pixelValues][]=3&tl[pixelValues][]=4&tl[pixelValues][]=5&tl[pixelValues][]=6&tl[pixelValues][]=7&tl[pixelValues][]=8&tl[pixelValues][]=9&tl[pixelValues][]=10&tl[pixelValues][]=11&tl[pixelValues][]=12&tl[legendKey]=monthly-spzgsa&tl[year]=2017&t[regionKey]=brazil&t[ids][]=8edd8cc7-e345-4541-a26d-37551e3628fa&t[divisionCategoryId]=213))
- mosqlimate_api/ - Contains two datasets of climate data obtained from the Mosqlimate datastore ([Mosqlimate API](https://api.mosqlimate.org/api/docs#/datastore/datastore_api_get_copernicus_brasil)):
  - climate_api_data_2016_2024.csv: Daily climatic data from 2016-01-01 to 2024-12-31, used for the main analysis
  - climate_api_data_aug_2003_jul_2004.csv: Daily climatic data from 2003-08-01 to 2004-07-31, used in the estimation of proper parameters of the birth rate, based on the work by de Barros, Honório and Arruda (2011)
- sivep/ - Daily cases of infection by malaria:
  - cumulative_manaus_cases_2016_2023.csv: Aggregated daily data on total cases of malaria occurring in Manaus from 2016-01-01 to 2024-12-29
  - malaria_vivax_YYYY_treated.csv: Daily notifications of malaria in Brazil, separated by year 
  - yearly_summary_2016_2023.csv: Summary of yearly data on total new cases occurring per year in Manaus,	average daily number of active cases, highest number of simultaneous active cases, cumulative number of cases by the end of the year
- trajetorias/ - Contains epidemiological and populational data gathered from the Trajetorias Project ([https://www.nature.com/articles/s41597-023-01962-1](https://www.nature.com/articles/s41597-023-01962-1) (Paper); [https://zenodo.org/records/7098053](https://zenodo.org/records/7098053) (Dataset)):
  - TRAJETORIAS_DATASET_Epidemiological_dimension_indicators.csv: Contains epidemiological data regarding type of disease, time period, location, residential zone, number of cases and incidence from the Trajetorias project
  - TRAJETORIAS_DATASET_Population_indicators.csv: Contains populational data regarding location, population in different time periods and estimated population 



The datasets may have undergone the following processing steps, as applicable:
- Data cleaning and consistency checks.
- Selection of observations within the study area and period.
- Temporal or spatial aggregation to obtain a common analytical resolution.
- Treatment of missing values and duplicate observations.
- Construction of derived variables used in the statistical analyses.

Data availability and reuse are subject to the terms and conditions of the original sources.

Datasets that are publicly available are referenced above. Data that cannot be redistributed are identified accordingly, together with instructions for obtaining them from their original providers, where permitted.

Please consult the original sources for applicable licensing and citation requirements.

