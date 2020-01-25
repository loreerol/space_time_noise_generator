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

By Lore and Sean!
