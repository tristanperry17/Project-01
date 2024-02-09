# Project-01
Severe Weather Impacts on NC Coastal Counties
Written by:

Justen Hix

Tristan Perry

Kayla Jehnzen

Zachary Pederson

This project seeks to independantly analyze the information suggested by the article below:
https://www.nrdc.org/stories/climate-change-floods-north-carolinas-housing-market#:~:text=As%20sea%20level%20and%20extreme,in%20debt%20and%20devalued%20homes

This article links climate change to rising sea levels, severe weather events, and consequently a potentially negative impact on populations and property values in three North Carolina counties. Notably, Dare, Hyde, and Carteret counties have been hit hard by these factors. Despite the increased risk to coastal properties, growth continues in these areas. 

The analysis in Main.ipynb in this repository pulls data from several sources in order to visualize relative metrics relating to the information in the source article.
Sources include:

Zillow
    https://www.zillow.com/research/data/
    Home Values (Single Family Homes) sorted geographically by county

OECD.org
    https://data.oecd.org/price/inflation-cpi.htm#indicator-chart
    CPI rates for consideration of inflation

NOAA
    https://tidesandcurrents.noaa.gov/sltrends/sltrends_station.shtml?id=8652587
    Data collected by NOAA Station 8652587, Oregon Inlet Marina, North Carolina
    Monthly mean sea levels with the average seasonal cycle removed

OpenWeatherApi
    https://openweathermap.org/api
    Data gathered for weather trends like windspeed of hurricanes and rainfall

OSBM.NC.gov & Census.gov
    https://linc.osbm.nc.gov/explore/dataset/census-county-to-county-migration/table/?disjunctive.area_name&disjunctive.year&disjunctive.external_area&disjunctive.external_county&sort=area_name
    Net migration data from county to county
    https://data.census.gov/table?g=040XX00US37_050XX00US37031,37055,37095
    Population data via US Census

The main script written for this project was merged together collaboratively from multiple notebooks. This program makes several uses of Pandas and Matplotlib functions, JSON for API calling, SKLearn, and hvplot for mapping. Data is read in from CSV format to create DataFrames, then cleaned when necessary, and visualized to produce graphs that showcase trends.

Findings from the analysis and visualization of these datasets, upon comparing property value and migration data with hurricane wind speed and precipitation data, show on a surface level that no statistically significant relations are present. Many factors beyond climate influence trends in demographics and property values, and more research and analysis would be needed to descern any potential relationships.

Challenges and limitations encountered during this project were mostly data based. Finding complete data sets that were concurrent for all three counties could have improved results. In particular, Hyde county, whose population is just a fraction of the other two counties, had limited property value and rainfall data available through the sources selected for this project. Timelines for datasets varied as well, making comparisons difficult. 

Improvements such as better data sourcing, using a smaller number of datasets that include more values as opposed to several different data sources, standardization of graphing techniques and formats, and longer timeframes for data sets may have added to the effectiveness of this project.
