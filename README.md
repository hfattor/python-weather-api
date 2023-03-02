# python-weather-api

Python script to create visualizions of the weather of over 500 cities of varying distances from the equator in Jupyter Notebook using Geoapify API and the geoViews Python library. 

## Weather-Py

Randomly generated geographic coordinates through Numpy. City information is pulled from the Citypy library. Weather information is pulled from the Open Weather Map API and populated into a dataframe, which is then exported into a .csv (contained in the outputs folder). 

Scatter plots were generated in Matplotlib to analyze weather data. These plots include:
<ul>
  <li>Latitude vs. temperature</li>
  <li>Latitude vs. humidity</li>
  <li>Latitude vs. cloudiness</li>
  <li>Latitude vs. wind speed</li>
</ul>

These graphs are exported into the output folder as .png files.

Linear regressions are calculated for each graph in the southern and northern hemisphere and the relationship between the data points is discussed in the notes of Jupyter Notebook file.

## Vacation-Py

Data from the previous exercise is imported from the .csv file. The cities are mapped through Hvplot. Personal weather preferences are applied to the data to narrow results. The Geoapify API is used to find the nearest hotel within 10,000 meters of the city coordinates. Results are added to a dataframe and mapped in Hvplot.
