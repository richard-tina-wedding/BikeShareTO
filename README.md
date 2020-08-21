# BikeShareTO

This is a project based on the Bike Share Toronto real-time GBFS data. Details and the real-time GBFS data can be found [here](https://ckan0.cf.opendata.inter.prod-toronto.ca/dataset/bike-share-toronto).

The GBFS data provides the locations of all bike share stations, the station capacity, and the real-time number of bikes available.

I wrote a script that records the timestamp and bike availability for all stations, and is recorded in an SQLite database.

The analysis studies the flow of bikes in and out of stations to understand where the bike traffic is going. 
