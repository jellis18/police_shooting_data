# Police Shooting Data With Census and Crime Data Covariates

The goal of this repository is to combine as much information at the county level to accompany 
police shooting databases as to facilitate predictions and data visualizations of police shooting data.

## Installation

1. Clone the repository
2. ``tar xzf data.tgz``
3. ``pip install -r requirements.txt``
4. Open Jupyter notebook (i.e., ``jupyter notebook combine_data.ipynb``)
5. Run notebook and all data will be created on the fly.

**Note:** Some of the police shooting data is not geocoded. If you wish to perform
this geocoding (otherwise the geocoded data is stored in ``derived_datasets``) then
you will need to have the [googlemaps](https://github.com/googlemaps/google-maps-services-python) python package installed along with a valid Google Maps API (follow the instructions in the link). Lastly, note that you will have to install ``googlemaps`` manually as it is not included in the ``requirements.txt`` file.

The datasets to be created are as follows (click link to download):

1. [Census data with various county-level features (2014)](https://raw.githubusercontent.com/jellis18/police_shooting_data/master/derived_datasets/county_level_census_data.csv)
2. [Police Shooting data from 2013-2016](https://raw.githubusercontent.com/jellis18/police_shooting_data/master/derived_datasets/combined_wp_mpv_shooting.csv)
3. [FBI county-level crime data (2014)](https://raw.githubusercontent.com/jellis18/police_shooting_data/master/derived_datasets/county_crime_data.csv)
4. [FBI county-level crime data summed by county and crime(2014)](https://raw.githubusercontent.com/jellis18/police_shooting_data/master/derived_datasets/summed_county_crime_data.csv)
5. [Combined county-level data with census, police shooting, and crime data](https://raw.githubusercontent.com/jellis18/police_shooting_data/master/derived_datasets/full_combined_county_data.csv)
6. [Police Shooting data with county-level crime and census covariates](https://raw.githubusercontent.com/jellis18/police_shooting_data/master/derived_datasets/shooting_data_with_county_covariates.csv)

Where possible intermediate datasets are downloaded directly from source. Otherwise they are stored in the ``datasets`` directory. 

Furthermore, all derived datasets will be stored in ``derived_datasets``.
