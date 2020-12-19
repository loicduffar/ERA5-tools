# ERA5-tools
#### Python scripts to download and view ERA5 climatologic data, as well as to extract time series (hourly to monthly data on many atmospheric, land-surface and sea-state parameters)

# Reanalysis ERA5-Land MONTHLY data from 1981 to present
## Download, Mapping and time serie extraction (from Copernicus "Climate Data Store")
MONTHLY Precipitations, runoff, potential evaporation, evaporation, temperature and snow stock.

- Data: https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-land-monthly-means?tab=overview
- ERA5-Land Data documentation: https://confluence.ecmwf.int/display/CKB/ERA5-Land%3A+data+documentation


author: Loïc Duffar https://github.com/loicduffar

### How to proceed ?
Run cells in order (red star <font color="red">*</font> indicates major steps):
- <a href=#section01>1)</a> <font color="red">*</font>Data download (only NetCDF format here, because more handy than GRIB format)
- <font color="red">*</font>IF the ERA5 file is already downloaded, start by the 2nd cell instead of the 1rst one
- <a href=#section02>2)</a> <font color="red">*</font>Customization, initialization and display netCDF file infos
- <a href=#section03>3)</a> <font color="red">*</font>Plot interannual average maps (annual and monthly interannual average) and save to files
- <a href=#section04>4)</a> <font color="red">*</font>Plot monthly timeserie for one pixel, and export it to excel file
- <a href=#section05>5)</a> Annual maps animation
- <a href=#section06>6)</a> Montlhy maps animation

- <a href=#section07>7)</a> Plot Maps over 12 months for a specific year (and one month map with basemap)
