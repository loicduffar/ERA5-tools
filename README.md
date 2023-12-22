<h1 align="center">ERA5-tools</center></h1>
<h4 align="center">Python scripts to download and view ERA5 climatologic data, as well as to extract time series (hourly to monthly data on many atmospheric and land-surface parameters)</center></h1>

### How to AUTHORIZE the execution of the download code on Windows ? (only once)
https://cds.climate.copernicus.eu/api-how-to

- If you do not have an account, please register on the CDS registration page
- Log in
- Copy the <a href="https://cds.climate.copernicus.eu/api-how-to">code with your personal key</a> (see below), into the file "USER/.cdsapirc" (in Windows environment)
(The file starting with a dot can be created using Notepad: "File> Save as> Type: All files> File name: .cdsfapirc"

    url: https://cds.climate.copernicus.eu/api/v2     
    key: {uid}:{api-key}
  
# Reanalysis ERA5-Land MONTHLY data (from 1981 to present)
## Download, Mapping and time serie extraction (from Copernicus "Climate Data Store")
MONTHLY Precipitations, runoff, potential evaporation, evaporation, temperature and snow stock.

- Data: https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-land-monthly-means?tab=overview
- ERA5-Land Data documentation: https://confluence.ecmwf.int/display/CKB/ERA5-Land%3A+data+documentation


author: Loïc Duffar https://github.com/loicduffar

### How to proceed ?
Run cells in order :
- <a href=#section01>1)</a> Data download (only NetCDF format here, because more handy than GRIB format)
- IF the ERA5 file is already downloaded, start by the 2nd cell instead of the 1rst one
- <a href=#section02>2)</a> Customization, initialization and display netCDF file infos
- <a href=#section03>3)</a> Plot annual and monthly interannual average maps (and save to files)
- <a href=#section04>4)</a> Plot monthly time series (for one pixel and for a possible polygon), and export them to excel file
- <a href=#section05>5)</a> Annual maps animation (OPTIONNAL)
- <a href=#section06>6)</a> Montlhy maps animation (OPTIONNAL)
- <a href=#section07>7)</a> Plot Maps over 12 months for a specific year (and one month map with basemap) (OPTIONNAL)

# Reanalysis ERA5-Land HOURLY data (from 1981 to present)
## Download, Mapping, daily/monthly aggregation and time serie extraction (from Copernicus "Climate Data Store")
HOURLY Precipitations, temperature, evaporation, runoff and other parameters.

- Data: https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-land?tab=overview
- ERA5-Land documentation: https://confluence.ecmwf.int/display/CKB/ERA5-Land%3A+data+documentation

author: Loïc Duffar https://github.com/loicduffar

### How to PROCEED ?
Run cells in order :
- <a href=#section01>1)</a> Data download (Download volume is limited by the server: you will have to adapt number of variables, the périod of time and the area and/or to split the request in several files)
- 1bis) Edit and run the 2nd cell, instead of the 1rst one IF the ERA5 file is already downloaded
- <a href=#section02>2)</a> Customization, initialization and display netCDF file infos
- <a href=#section03>3)</a> Plot maps by hour/day/month and interannual average
- <a href=#section04>4)</a> Plot and export dailly time serie for one pixel and for a possible polygon
- <a href=#section05>5)</a> Animation maps by month, day and hour (OPTIONNAL)
- 5bis) Animation maps by day and hour OVER A SELECTED PERIOD OF TIME. (OPTIONNAL: Use this cell instead of the one above if the navigation through the hourly data is difficult because of a file covering a very long duration; 10 years for example).

<img src="https://github.com/loicduffar/ERA5-tools/blob/main/out/ERA5-Land%20monthly%20averaged%20total_precipitation%201981-2020%20SRI%20LANKA%20BATTICALOA_Annual.png" width="20%"></img>
<img src="https://github.com/loicduffar/ERA5-tools/blob/main/out/ERA5-Land%20monthly%20averaged%20total_precipitation%201981-2020%20SRI%20LANKA%20BATTICALOA_Monthly.png" width="40%"></img>
<img src="https://github.com/loicduffar/ERA5-tools/blob/main/out/ERA5-Land%20monthly%20averaged%20total_precipitation%201981-2020%20SRI%20LANKA%20BATTICALOA_Monthly%20Time%20serie.png" width="60%"></img>
<img src="https://github.com/loicduffar/ERA5-tools/blob/main/out/ERA5-Land%20monthly%20averaged%20total_precipitation%201981-2020%20SRI%20LANKA%20BATTICALOA_Annual%20Correlation.png" width="60%"></img>
