# CorData
This is a MatLab App that fetches corona-19 data from [data.world](https://data.world/covid-19-data-resource-hub/covid-19-case-counts) (Johns Hopkins data). 

## Component
A MatLab [app file](CorData.mlapp) and a [config](app_config.m) file. Pull these two files to a folder.

The config file contains configuration data for tuning the App.

## Usage
Before you can use this App the first time, you need to edit the 
# Config file
There is a one-time setup step to get a free api key from data.world.
Get a free data.world apikey first. Goto [data.work](https://data.world/covid-19-data-resource-hub/covid-19-case-counts).
![data_world](images/data_world.png)
Click "Join to view this file". 
Select one way to join data.world from the popped up dialog. 

Once you can sign, you get a free apikey. 

Go back the same [page](https://data.world/covid-19-data-resource-hub/covid-19-case-counts), click the download button for the "COVID-19 Cases.csv" file. Select "Share URL", your apikey will be shown:
![api_key](images/sharedlink.png)
