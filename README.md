# COVID-19 Case/Rate Data Visualization

This project maps available COVID-19 information (2020 data) over the Contiguous United States at the county level to showcase how the diseases spread and the largest hotspots. In these interactive maps, COVID-19 Case (quantity) and Rate (cases per 1,000 people) data are visualized in two different mapping techniques.

### Map 1: COVID-19 Rate Map (Choropleth)

The first map is a Choropleth visualization of COVID-19 Rates measured in counts per 1,000 people. The data is broken up into 8 ranges, and each one is colored to signify how high of a rate exists in a given county.

[Click here to view the COVID-19 Rate Map](https://masonhowes.github.io/covid_case_visualization/map1.html).

![Image of the Choropleth COVID-19 Rate spread](img/map1.png)

The primary function of this visualization is to showcase the different counties across the country that experienced the highest COVID-19 transmission rates. At a Choropleth map, it is easy to see these high-transmission areas as noted by the colorschemes without having to get too focused on the number of cases. This is important for individuals to be able to easily see what areas of the country are best to be avoided in order to help stop the spread of the virus.

The user is able to hover over a given county on the map and the window in the top left of the screen will inform the user the rate of COVID in said county. The bottom left of the map includes the Legend which defines the scale that the colors are based on.

### Map 2: COVID-19 Case Map (Proportional Symbol)

The second map is a Proportional Symbol visualization of COVID-19 Counts in each county of the Contiguous United States. The symbols are based around 3 different levels and said levels are indicated by the size of the dot that houses their information.

[Click here to view the COVID-19 Case Map](https://masonhowes.github.io/covid_case_visualization/map2.html).

![Image of the Proportional Symbol COVID-19 Case quantities](img/map2.png)

The primary function of this visualization is to inform the user of the areas that contain the highest counts of COVID-19 at the county level. This visualization is purely numerical and doesn't use a formula to calculate its value like the rates map did.

The user is able to click on a given dot and they will be informed as to what the number of cases in a given county was. In the bottom right of the screen a legend exists that outlines what each sized dot signifies.

### About this project

This project uses libraries hosted by The New York Times, specifically their [covid-19-data-bot](https://github.com/nytimes/covid-19-data/blob/43d32dde2f87bd4dafbb7d23f5d9e878124018b8/live/us-counties.csv). The population data in this map is from the [2018 ACS 5 year estimates](https://data.census.gov/table/ACSDP5Y2018.DP05?g=0100000US$050000&d=ACS%205-Year%20Estimates%20Data%20Profiles&hidePreview=true), and the US county shape files from the [U.S. Census Bureau](https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html).

The viewable map is created thanks to [MapBox](https://www.mapbox.com/), and the color scales used in the Proportional Symbol map were provided by [ColorBrewer](https://colorbrewer2.org/#type=sequential&scheme=OrRd&n=3). In order to minimize filesize, [mapshaper](https://mapshaper.org/) was used to simplify map data.

I would like to acknowledge my professor Bo Zhao for the bulk of the coding work on this project, and Steven Bao for data processing help.
