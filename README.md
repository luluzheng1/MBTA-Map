# RedLine Updates
RedLine Updates is a web page that shows all the Massachusetts Bay 
Transportation Authority Red Line subway train stations on a map along with
eachstation's real-time schedule of upcoming trains. 

## APIs
This web application uses the Google Maps API to display a map that spans the 
entire page and the MBTA API to provide real-time data on subway schedules. 
The web page is hosted in LocalHost.

## Features
* Red pins on the location of red line stops in map
* Map centers at South Station initially 
* A red line shows the path of Red Line and connects all the stations
* Geolocation
	- Determines the user's location
	- Places a pin at that location
	- The pin is Google's default pin
	- Once geolocation is determined, map centers at user's location 
* Information window pops up when the user's pin is clicked
	- Displays name of and distance to the closest red line station 
	- Renders a line connecting the user's pin to that station
* Information window pops up when a station's pin is clicked
	- Displays the arrival time (northbound and southbound)
  	  of upcoming trains

## Acknowledgement
I used the classic Haversine Formula to calculate the distance between 
two geopoints, which is provided and analyzed at [Haversine Formula](http://www.movable-type.co.uk/scripts/latlong.html).
I also referred to the JavaScript implementation of the 
[Haversine Formula](https://stackoverflow.com/questions/14560999/using-the-haversine-formula-in-javascript)
on Stack Overflow. 

