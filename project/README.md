### Goal of project
This project aims to explore the impact of vaccination rate on COVID-19 cases and death and unemployment rate in Macomb County, Michigan. The analysis begins with the data acquisition procedure of combining county specific raw data from three different sources into aggregated.xlsx. The data combination process is done manually using Microsoft Excel. That is perceived as the best method for this step as the size of the data is not big. 

After data cleaning and manipulation, three time series are assessed. More specifically, three relationships will be explored in this analysis:  
1. COVID-19 cases and deaths vs unemployment rate  
2. COVID-19 cases and deaths vs vaccination rate  
3. Unemployment rate vs vaccination rate  

[Granger causality test](https://en.wikipedia.org/wiki/Granger_causality) and [Pearson correlation test](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient) are used to explain whether the time series are correlated to one another. Results and explanation are included in the report in this repo. 

### Data source
1. [Kaggle repository of John Hopkins University COVID-19 data](https://www.kaggle.com/datasets/antgoldbloom/covid19-data-from-john-hopkins-university): This data repo is updated on a daily basis and contains the confirmed and death cases of COVID-19.  
2. [Michigan State Vaccination Record](https://www.michigan.gov/coronavirus/resources/covid-19-vaccine/covid-19-dashboard): Michigan state uploads on daily basis the number of vaccination administered in Michigan by county. The data is available since December 2020.  
3. [The US Bureau of Labor](https://fred.stlouisfed.org/series/MIMACO9URN): The US BLS publishes monthly unemployment rate data by county.  
4. [CDC dataset of masking mandatory ](https://data.cdc.gov/Policy-Surveillance/U-S-State-and-Territorial-Public-Mask-Mandates-Fro/62d6-pm5i): This data contains information about implementing mask mandate in various counties in the US.


### License
MIT Open Source: https://opensource.org/licenses/MIT         

### Files and data
- final_project.ipynb contains the data manipulation, visualisation and statistical analysis process during the research project. Comments and analysis are included as part of mark down in the notebook.  
- COVID_cases_deaths.png shows the trend of monthly aggregated COVID-19 cases and deaths in Macomb County, Michigan from December 1, 2020 to October 30, 2022. 
- monthly_unemployment.png shows the trend of monthly unemployment rate(%) in Macomb County, Michigan from December 2020 to October 2022.  
- monthly_vaccination.png shows the trend of monthly aggregated vaccination rate in Macomb County, Michigan from December 2020 to October 2022.  

