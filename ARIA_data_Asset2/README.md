# General description
Datasets used to train a simplified Deep Learning model for estimating wind speed at hourly basis. 

### Content

`target_data.csv` file is a csv containing wind speed data from an existing wind farm located in the Apulia region, Italy. Data has been masked for anonymisation purposes by aggregating the 10-minute recordings into hourly values by using the median wind speed during the hour and by scaling the resulting values. Temporal range is Jan 2021 - Dec 2021 at hourly basis. It has been used as target feature for wind speed estimation. 

`feature_data.csv` is a csv file containing time-series data from the ERA5Land reanalysis, sourced from the CDS repository. It is instrumental for the training and testing of the simplified model. Temporal range is Jan 2021 - Dec 2021 at hourly basis.

#### Feature Data Contents

The `feature_data` CSV file encompasses several key meteorological elements, detailed as follows:

- **Wind Speed**: Rather than being a primary observation, this value is computed based on the U and V wind components.
- **Temperature at 2 Meters**: This is the temperature recorded 2 meters above the ground.
- **Surface Pressure**: This metric indicates the atmospheric pressure at the Earth's surface.

#### Source

The data has been retrieved from the [CDS Repository](https://cds.climate.copernicus.eu/cdsapp#!/home), stemming from the ERA5Land reanalysis. ERA5Land is a global land-surface dataset at 9 km resolution, updating the ERA5 reanalysis data with a finer, more detailed grid on land areas.

### License
Creative Commons Attribution 4.0 International License
