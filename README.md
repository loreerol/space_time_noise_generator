# Space Time Noise Generator

This App will take in GPS data of the user and use various APIs to gather information about the user's environment and create a unique sound piece based on the place and time the user is currently occupying. This piece will change over time as the data changes.

_Ideas for data we'd like from an API:_
+ Weather - Pollution
+ Temperature, humidity, wind speed and direction 
+ Tectonic action 
+ Sun rise sunset
+ Pressure 
+ Precipitation 
+ Surf forecast
+ Moon phase
+ Holiday/off work day/weekend
+ Possibly light sensor - look into 
+ Season
+ Traffic
+ Time of day - day of week

_The plan_
1. Research APIs, find out what data we can actually work with
2. Create the architecture - layers: API, translation. Generator classes
3. Actually get the API data working and displaying in browser
4. Pull in the Tone.js library and start associating data and sounds/effects etc.
5. Add in some variety/complexity using algorithms - Neo-Riemannian theory, Markov chains, Bernoulli distribution
6. Design the UI to show data and possibly have some user controls 

_APIs - It’s possible that there are better APIs out there, but we can start with these_

Open Weather - Current Weather API https://openweathermap.org/current
- Current weather
- Daily high/low
- Pressure
- Humidity
- Wind speed/degrees
- Cloud cover
- Sunrise and sunset
- Timezone

Air Quality API https://aqicn.org/api/
- Air quality and pollution level (Air quality index)

Earthquake catalog https://earthquake.usgs.gov/fdsnws/event/1/
- You can specify a radius around a location
- Whether an earthquake is currently happening inside the radius and the severity

Tides API https://www.worldtides.info/apidocs
- Sea conditions /tides 

Moon phase API https://www.mooncalc.org/#/49.495,11.073,3/2020.01.26/16:00/1/0
- Has moonrise moonset and phase
- There are also algorithms we can use without an API call for this info

Traffic https://developer.here.com/documentation/traffic/dev_guide/topics/what-is.html
- Traffic incident data
- Traffic flow data

_Special conditions users may have:_
- If the user is over water, check the sea conditions, tides
- If the user is in a city, check how congested traffic is, air quality
- If the user is close to the equator
- Elevation, perhaps they are very high or low?
- If it’s the evening - is the night clear? What is the phase of the moon, how high is it?

By Lore and Sean!
