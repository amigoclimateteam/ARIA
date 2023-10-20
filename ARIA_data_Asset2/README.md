# General description
Datasets used to train the ML model for estimating wind speed at hourly basis. 

### Content

`feature_data.csv` file is a csv containing wind speed data from a station located at Max-Plack Institute https://www.bgc-jena.mpg.de/wetter/Weatherstation.pdf. Temporal range is Jan 2020 - Dec 2021 at hourly basis. It has been used as target feature for wind speed estimation. 

`feature_data.csv` is a csv file containing time-series data from the ERA5Land reanalysis, sourced from the CDS repository. It's instrumental for our model's training phase. Temporal range is Jan 2010 - Aug 2023 at hourly basis.

#### Feature Data Contents

The `feature_data` CSV file encompasses several key meteorological elements, detailed as follows:

- **U Component of Wind**: This represents the west-east wind component, indicating the intensity of the wind moving from west to east.
- **V Component of Wind**: This signifies the south-north wind component, indicating the intensity of the wind moving from south to north.
- **Wind Speed**: Rather than being a primary observation, this value is computed based on the U and V wind components.
- **Temperature at 2 Meters**: This is the temperature recorded 2 meters above the ground.
- **Surface Pressure**: This metric indicates the atmospheric pressure at the Earth's surface.

#### Source

The data has been retrieved from the [CDS Repository](https://cds.climate.copernicus.eu/cdsapp#!/home), stemming from the ERA5Land reanalysis. ERA5Land is a global land-surface dataset at 9 km resolution, updating the ERA5 reanalysis data with a finer, more detailed grid on land areas.

### License
Creative Commons Attribution 4.0 International License
