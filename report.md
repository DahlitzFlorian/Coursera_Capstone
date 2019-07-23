# Final Report: The Similarities between New York and Hamburg

## Introduction

As the de facto metropole region of Germany concerning the connection to overseas markets, Hamburg plays an important role for the whole european continent.
What New York is for the financial community in the US, Hamburg is for the oversea trade community in europe.
With that said an interesting question arises: How do the people live in both cities?
How similar or dissimilar are they?

This short report tries to answer the questions at hand using available data provided by [Foursquare][Foursquare].


## Data

To be able to answer the questions mentioned in the first section, location data from [Foursquare][Foursquare] will be used.
Please note, that no additional data sources will be used.
The data will be accessed through Foursquares API.
It is available in JSON format.


## Methodology

In order to answer the questions formulated in the introductions section with the data from [Foursquare][Foursquare], an analytical approach is used.
Therefore, location data for both cities, Hamburg and New York, is queried from Foursquare and prepared afterwards.
In the next step k-means clustering is used to cluster neighbourhoods of each city and compare them.
Lastly, both cities clusters are compared and evaluated to show how similar or dissimilar they are.


## Results

The New York City results or in particulat the Manhattan results were presented in the `new-york.ipynb` notebook.
If you have a look at the five clusters, which were generated, you can see, that Manhatten is a quite heterogen borough.
All the neighborhoods are nearly equally distributed over the five clusters.

However, if you have a look at the final map for the city of Hamburg, you can see, that Hamburg itself is a quite homogen city.
We used only three clusters as not so many neighborhoods exist as in Manhattan.
There is only one neighborhood in the first and third clusters, whereas all other neighborhoods are in the second cluster, which means, that they are quite similar.
Even if we use five clusters like for Manhatten, there exists only one neighborhood per cluster except one covering all other neighborhoods.

You can view the maps either in the notebooks or in the `presentation.pptx`.


## Discussion

A major problem in comparing New York City (in this case Manhattan) and Hamburg is, that Hamburg is smaller and has fewer neighborhoods, which makes it harder to cluster them and makes it more likely to have a homogen city.
Furthermore, New York is a worlds city whereas Hamburg is mostly (only) important for Germany (and Europe).


## Conclusion

Finally, comparing both cities shows, that Hamburg is a more homogen city with the neighborhood *Altona* as an outlier (Altona is somehow very special in Hamburg - people from Hamburg know that).
In contrast New York City or in this case Manhattan is a very heterogen city.
The cause might be the bigger number of people as well as the fact, that it's a world city.


[Foursquare]: https://foursquare.com/
