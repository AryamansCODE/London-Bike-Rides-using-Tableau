# London-Bike-Rides-using-Tableau

This project involves the analysis of a bike-sharing dataset sourced from multiple platforms. The data spans from January 1, 2015, to December 31, 2016, and includes various weather conditions and calendar information.

## Project Repository

All relevant files for this project are stored in the GitHub repository:

- **Original Dataset**: `original_dataset.csv`
- **Jupyter Notebook**: `DataExtractionManipulation.ipynb`
- **Transformed Dataset**: `london_bikes_final.xlsx`
- **Tableau Dashboard**: `BikeRides Analysis London final.twbx`
- **Dashboard Screenshots**: `Dashboard_Screenshots/`

## Data Sources

1. **TfL Open Data**:
    - [Cycling Data](https://cycling.data.tfl.gov.uk/)
    - Contains OS data © Crown copyright and database rights 2016
    - Geomni UK Map data © and database rights [2019]

2. **Weather Data**:
    - [freemeteo.com](https://freemeteo.com)

3. **Holiday Data**:
    - [UK Bank Holidays](https://www.gov.uk/bank-holidays)

## Dataset Overview

- **Time Period**: 1/1/2015 to 31/12/2016
- **Total Rows**: 17,414
- **Total Columns**: 10

### Columns and Metadata

The dataset includes the following columns: `timestamp` (timestamp field for grouping the data), `cnt` (the count of new bike shares), `t1` (real temperature in Celsius), `t2` (feels-like temperature in Celsius), `hum` (humidity in percentage), `wind_speed` (wind speed in km/h), `weather_code` (category of the weather), `is_holiday` (boolean field: 1 if holiday, 0 if not), `is_weekend` (boolean field: 1 if weekend, 0 if not), and `season` (category field for meteorological seasons: 0: spring, 1: summer, 2: fall, 3: winter).

### Weather Code Descriptions

The weather codes are described as follows: `1` (Clear/mostly clear, some haze/fog), `2` (Scattered clouds/few clouds), `3` (Broken clouds), `4` (Cloudy), `7` (Rain/light rain shower/light rain), `10` (Rain with thunderstorm), `26` (Snowfall), and `94` (Freezing fog).

## Data Transformations

1. **Extraction**:
    - Extracted data from the zip file using NumPy and Pandas.

2. **Data Understanding**:
    - Analyzed the shape and basic information of the dataset.
    - Analyzed value counts in the 'season' and 'weather_code' columns.

3. **Data Cleaning**:
    - Renamed columns for clarity.
    - Used metadata to replace code values in 'season' and 'weather_code' with descriptive labels.

4. **Data Conversion**:
    - Converted the final dataset to an Excel file for further analysis.

## Visualization and Analysis

- Imported the transformed dataset into Tableau.
- Developed dashboards to visualize various aspects of the data, such as:
    - Sum of bike sharing hours.
    - Wind speed vs. temperature heat map using a moving average graph to select the time period.
    - Added floating charts when hovered over the heatmap of wind and temperature. These floating charts depict hourly use of bikes and the type of weather during that period.

## Contact

For any queries or further information, please contact me at: aryamanmalik04@gmail.com

---

Feel free to modify and expand upon this template as needed for your specific project requirements.
