The weather study includes two parts, the first is to determine if the weather is better as you get closer to the equator.  Besides utilizing scattor plots to vislualize the information, the data was grouped into their corresponding hemispheres with each weather element and analyzed using linear regression and R scores to determine their validity in the study. The city and temperatures were plotted using a heatmap in gmaps to view our data globally.  An additional study to determine the best places to vacation based on specific weather conditions was used to create another map.  This data was then joined with an additional API call to https://maps.googleapis.com/maps/api/place/nearbysearch/json to locate a hotel within 5000 meters of the city coordinates and put the information into a pop-up when the mouse is moved over the map.  

Is it warmer closer to the Equator?

Weather Study that gathers weather data from API calls that match randomly generated longitude and latitudes and plots them into various scatter plots to see if the weather is better as you get closer to the equator.  The weather elements used to determine this study included temperature, humidity, cloudiness and windspeed compared to a cities latitude.  

The study began with generating 1500 random longitude and latitudes coordinates which were mapped to the closest city using the citipy library to capture the nearest cities actual coordinates. The data was loaded into a dataframe along with columns to store the different weather elements.  An API call was made to http://api.openweathermap.org/data that matched our actual coordinates.  The weather elements were put in the dataframe so the data could be plotted.  Each of the weather elements was plotted individually.

A copy of the data created and used in the study is located in Outputs/Weather_Data_API.csv.   Copies of the charts comparing the various weather elements and the corresponding latitude of the cities are located in the Outputs folder and is identified by the title of the png file. A copy of the linear regression and R score analysis for each hemisphere is located in the weatherpy.ipynb file.

Best Vacation Spots 

This study used the data from the previous analysis that was reduced using specific weather element conditions to find the ideal vacation spot.  The conditions included temperatures between 50-62, 80% cloudiness and less than 15 miles an hour windspeed. The information was used to create a layered gmap with a marker layer containing the Country, City and Hotel Name.


