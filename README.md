The weather study includes two parts, the first is to determin if the weather is better as you get closer to the equator.  Besides usitulizing scattor plots to vislualize the information, the data was grouped into their corresponding hemispheres and analyzed using linear regression and R scores to determine the validity of our study. The city and tempateratures were plotted using a heatmap in gmaps to view our data globally.  An additional study to determine the best places to vacation based on specific conditions was created.  This data was then joined with another API call to gether information on 

Is it warmer closer to the Equator?

Weather Study that gathers weather data from API calls that match randomly generated longitude and latitudes and plots them into various scatter plots to see if the weather is better as you get closer to the equator.  The weather elements used to determine this study included temperature, humidity, cloudiness and windspeed compared to a cities latitude.  

The study began with generating 1500 random longitude and latitudes coordinates which were mapped to the closest city using the citipy library to capture the nearest cities actual coordinates. The data was loaded into a dataframe along with columns to store the different weather elements.  An API call was made to http://api.openweathermap.org/data that matched our actual coordinates.  The weather elements were put in the dataframe so the data could be plotted.  Each of the weather elements was plotted individually.

A copy of the data created and used in the study is located in Outputs/Weather_Data_API.csv.  Copies of the charts comparing the various weather elements and the corresponding latitude of the cities.


