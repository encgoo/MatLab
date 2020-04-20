# CorData
This is a MatLab App that fetches corona-19 data from [data.world](https://data.world/covid-19-data-resource-hub/covid-19-case-counts) (Johns Hopkins data). 
![app](images/show_data.png)

## Component
A MatLab [app file](CorData.mlapp) and a [config](app_config.m) file. Pull these two files to a folder.

The config file contains configuration data for tuning the App.

## Usage
Before you can use this App the first time, you need to edit the config file.
### Config the App
There is a one-time setup step to get a free api key from data.world first.
Go to [data.work](https://data.world/covid-19-data-resource-hub/covid-19-case-counts).
![data_world](images/data_world.png)
Click "Join to view this file". 
Select one way to join data.world from the popped up dialog. 

Once you signed in, you get a free apikey. 

No go back the same [page](https://data.world/covid-19-data-resource-hub/covid-19-case-counts) above, and click the download button for the "COVID-19 Cases.csv" file. Select "Share URL", your apikey will be shown:
![api_key](images/sharedlink.png)
Now use an text editor to edit the app_config.m you pulled from git and put your apikey there.
![api_key_config](images/apikey.png)

### Start the App
Just open CorData.mlapp from MatLab. Make sure you change your working directory to the folder of CorData.mlapp so MatLab can find the app_config.m file. Run the App inside MatLab.

![cordata](images/cordata.png)

Click "Refresh" to start downloading data and show. Note it takes a while to download the csv file (~70MB) and process the data.

![showing_data](images/show_data.png)

Note that the checkbox of "show normal distribution fit" has been checked to show the red line. It tries to fit the curve into a normal distribution. Adjust the standard deviation to see different result.

Also select other country/state to view other data.

## Summary
The whole app contains only ~250 lines handwritten code, plus ~100 lines auto-generated code. This shows the strong support from MatLab that greatly simplified the development job.
 

