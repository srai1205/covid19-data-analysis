# covid19-data-analysis
Create a Data Warehousing solution for covid-19 data of europe region. we had ingest covid-19 cases, deaths, hospitalization and testing data from 
European Centre for Disease Prevention and Control website(https://www.ecdc.europa.eu/en/covid-19/data).we have transfromed the data using Azure Data Factory(ADF) and Azure Data Bricks(ADB).
Following are the transfromations carried out on data:-

1) Cases and Deaths data transformation

![transformation_cases_and_deaths](https://user-images.githubusercontent.com/43174715/191204388-6fedc32c-89a5-4251-b61c-54550e565505.png)

2) Hospitalization data transformation

![transformation_hospital_data](https://user-images.githubusercontent.com/43174715/191204534-4941c328-04fb-4232-977e-baaa3b95f72f.png)

3) Testing data transformation 

Testing raw data image.
![Testing_raw](https://user-images.githubusercontent.com/43174715/191208215-902bed9f-454c-4391-b142-7bdb25db915b.png)

transformations:- Get start data and end data of a week from dim_date lookup file.Fetch 2 digit and 3 digit country code from dim_country table.

we copy the transformed data in Azure SQL Database using ADF copy activity. Analyzed the transfromed data to create Power BI dashboard for trends based on countries and testing. 
Following are the screenshot of dashboard:-

1) Trends of total cases, deaths, Hospital and ICU occupancy for countries in Europe:-

![Trends](https://user-images.githubusercontent.com/43174715/191199305-e463fc3d-63ad-4ba2-8da5-eb8f39365868.png)

2)Compare different countries based covid-19 cases and deaths:-

![Trendsbycountries](https://user-images.githubusercontent.com/43174715/191199666-f3a03c3b-e95f-4848-8c1d-7c1536081440.png)

3)Compare countries by testing and country's testing and confirmed cases data.

![Testing](https://user-images.githubusercontent.com/43174715/191200124-a11132bf-02b2-4fc2-94b0-0a273d6f65d9.png)

