# BikeShareTO

This is a project based on the Bike Share Toronto real-time GBFS data. Details and the real-time GBFS data can be found [here](https://ckan0.cf.opendata.inter.prod-toronto.ca/dataset/bike-share-toronto).

The GBFS data provides the locations of all bike share stations, the station capacity, and the real-time number of bikes available.

I wrote a script that records the timestamp and bike availability for all stations every 10 minutes, and the data is recorded in a SQLite database.

The analysis studies the flow of bikes in and out of stations to understand where the bike traffic is going. I performed an analysis of the before-work hours and start-of-work hours to see how the traffic clusters to busy work locations like on University Ave (where the hospitals are) and by the Financial district. The city of Toronto has implemented the ActiveTO program over the weekends where there are road closures to encourage bike riding. This impact is seen by the amount of ridership along the Lakeshore bike stations.

A folium map was made to visualize the flow, with the size of the marker representing the fractional change in capacity, and the red markers represent stations that had a net flow of bikes out, and the green markers had a net flow of bikes in. Additional details are shown in the tooltip when the mouse is hovered over a marker.
