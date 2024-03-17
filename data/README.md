## Data files for COMM2550 Data Project

This folder contains the raw and cleaned data files used in our project.

1. `google_trends`
    * This folder contains one csv file
    * The csv contains the Google Trends search popularity data for nine search terms, for a duration of 10 years between 2012 and 2022, with an interval of 1 week
    * This data was collected from Google Trends, using the Python package `pytrends`
        * See `data_analysis/data_cleaning/trends_dl.ipynb` for full details of how this data was obtained

<br>

2. `weather`
    * This folder contains two csv files
    * Both files contain information for various weather measures
    * `weather.csv` contains daily information for a set of weather measures:
        * temperature (minimum, maximum, mean)
        * apparent temperature (minimum, maximum, mean)
        * sunrise and sunset time
        * shortwave radiation energy (sum; in mega-Joules per square meter)
        * precipitation amount (sum; in millimeters)
        * rain amount (sum; in millimeters)
        * number of hours of precipitation
        * wind speed (maximum; in kilometers per hour)
        * wind gusts (maximum; in kilometers per hour)
        * wind direction (in degrees)
        * evapotranspiration rate (mean; in millimeters)
    * `weather2.csv` contains hourly information for a separate set of weather measures:
        * relative humidity (mean of current hour; in percent)
        * direct radiation amount (mean of preceding hour; in Watts per square meter)
        * wind speed (mean of current hour; in kilometers per hour)
    * All of these data were collected from Open Meteo's public API, which can be found at [this link](https://open-meteo.com/en/docs/historical-weather-api)

<br>

3. `weekly_disease_bulletin`
    * This folder contains one csv file and one metadata file
    * The csv file contains the data for the number of reported cases of a full list of infectious diseases in Singapore, for a duration of 10 years between 2012 and 2022, with an interval of 1 week
    * The metadata file contains the original metadata and related information that comes packaged with the downloaded dataset
    * This data was downloaded from Singapore's [official open data repository](data.gov.sg)

<br>

4. `cleaned`
    * This subfolder contains three csv files
    * These csv files are the cleaned versions of the datasets that were obtained
    * For details of the data cleaning process, see the notebooks in `data/data_analysis/data_cleaning`
    * Each of these cleaned csv files are named according to their respective original datasets