## Azure-Olympic-Games-Analysis

## Description
The Tokyo Olympic Data Engineering Project is a comprehensive data engineering solution that utilizes various Azure services, including Azure Databricks, Azure Data Lake, Azure Synapse Analytics, and Azure Data Factory. This project aims to collect, process, analyze, and visualize data related to the Tokyo Olympic Games.




## Architecture
<img src="/imgs/Tokyo Olympic Data Analytics Data Engineering Project.JPG" width="50%">

Data Source :- This contains the details of over 11,000 athletes, with 47 disciplines, along with 743 Teams taking part in the 2021(2020) Tokyo Olympics.
This dataset contains the details of the Athletes, Coaches, Teams participating as well as the Entries by gender. It contains their names, countries represented, discipline, gender of competitors, name of the coaches.
Used a GitHub repository with CSV files

Data Factory :- Connected the data sources to Azure Data Factory, ingested using the HTTP API.

Azure Data Lake Gen2 (for data storage): Connected Azure Data Factory to an Azure Data Lake Gen2 for storage.

Azure DataBricks: Connected from Azure Data Lake Gen2 to Azure DataBricks for data transformation process with PySpark.

Azure Data Lake Gen2: After Azure DataBricks, load the transformed data back to the Data Lake Gen2.

Azure Synapse: From the Data Lake, make a connection to Azure Synapse and used SQL scripting there to receive and make other analytics.

Analytics Tools: Lastly, this is not within the scope of data engineering, but the ground work has been laid out to do the dash boarding with Tableau, PowerBI, and Looker.



## Visualization
<img src="/imgs/data_factory_copy.JPG" width="50%">
<img src="/imgs/azure_synapse_analytics.JPG" width="50%">
<img src="/imgs/no_athletes_each_country.JPG" width="50%">
<img src="/imgs/total_gold_medal_countries_greater_than 20.JPG" width="50%">
<img src="/imgs/total_medal_won_ech_country.JPG" width="50%">

