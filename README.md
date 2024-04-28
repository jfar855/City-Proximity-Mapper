# City-Proximity-Mapper
City Proximity Mapper is a sophisticated Python tool designed to determine the nearest cities to a specified geographic coordinate, with optional filters for minimum population and limiting the number of results. This utility reads city data including location and population, and provides fast, accurate proximity searches using Vincenty's and Haversine formulas.

## Features

- **Geographic Search**: Enter latitude and longitude to find nearby cities.
- **Population Filtering**: Option to specify a minimum population for the cities returned.
- **Result Limitation**: Ability to limit the number of cities returned.
- **Precision Calculations**: Utilizes Vincenty's formula for high-accuracy distance calculations with Haversine as a fallback.

## Usage

Run the script from the command line, specifying the data file and geographical coordinates. You can also add optional parameters for population and number of results:
EX: python cities.py city_data.txt 38.9897 -76.9378 -p 50000 -n 5
- This command will search for up to 5 cities near the coordinates 38.9897, -76.9378 with populations of at least 50,000.

## Data Format
The city_data.txt file should contain tab-separated values with the following format for each city:
CityName\tLatitude\tLongitude\tPopulation
EX: Marijampolė\t54.55991\t23.35412\t47613
