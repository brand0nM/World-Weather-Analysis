# World-Weather-Analysis
## Project Overview
We've been tasked with creating a PlanMyTrip app; The user will input their desired temperature range and the app will filter those results, outputing a map of cities with hotels. 

### Purpose
Use python's random package to create a list of 2000 randomized GCS coordinates. Then retrieve the city name- if location is a city- and the local weather data from a rest API. Next ask the user to filter the results based on their ideal temperature range in degree's farenheight, and create a new dataframe with a close hotel in that city (using Google Map's api). Finally create a route for our vacation between the selected hotels, and list their info in markers on the map.

---
## Analysis
From 2000 randomized coordinates, first append each city and their local weather data to a new dataframe, then print the amount that weren't cities. Since we are using a free version of these API's the amount of request per minute is limited; hence we must first populate a data frame with more city info- use more randomized coordinates (100k)- or we could upgrade to the premium API version.
<br />

<img width="1436" alt="Screen Shot 2022-04-24 at 1 38 22 PM" src="https://user-images.githubusercontent.com/79609464/164993535-0a0bb7d5-62c8-4585-bdf4-f6e5ec50c3df.png">

### Average Temperatures between 70-82 
Prompt our user to enter their desired temperature range and create a new filtered data frame; then append hotel names to the data frame.
<br />

<img width="1439" alt="Screen Shot 2022-04-24 at 1 34 59 PM" src="https://user-images.githubusercontent.com/79609464/164993446-b4ce00dc-c663-4bff-ba36-055f6bc7303b.png">
<br />

Plot a map of travel desination for the user to choose from.
<br />
<img width="1415" alt="WeatherPy_vacation_map" src="https://user-images.githubusercontent.com/79609464/164992988-82ea777f-3db0-4b4c-98f1-2725dcc04c04.png">

### Madagascar Vacation
Our user has decided on Madagascar. From the hotels they've selected we output a map with a path between hotels and markers with a quick synopsis.
<br />

<img width="1100" alt="Screen Shot 2022-04-24 at 1 26 40 PM" src="https://user-images.githubusercontent.com/79609464/164993141-ab71b1bd-a129-4aaa-99b5-8dc401261812.png">


### Challenges and Difficulties
Since we are using the free version of the weatherdata API it takes around 40 minutes to populate our data frame; further 2000 cities is not a lot of datapoints. To make this analysis more complete we should try to add every city from every country to our dataframe. Another way to improve this model is to create a different function that takes in a city or country name, and finds its local weather data and the top rated hotels in the area; This modification would require unlimited packages with both API's though because they limit the amount of requests. 

---
## Summary
We were able to create a PlanMyTrip app that takes in a user's specified temperature range and outputs a map with hotels for the user to choose from. 

---

