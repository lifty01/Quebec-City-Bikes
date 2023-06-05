# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The project consisted as a way to put into practice everything learned in Python so far and build a statistical model to find a link between two variables. We wrote code to request data from different APIs and parsed through the data, using a few built-in packages to select and filter out the desired data to put it into dataframe(s), and then extracting some of the data to make graphs, before finally running the selected data into a statistical model to check for the validity of the model based on the data.
I personally selected for the number of parks within a certain range when comparing them to specific bike stations.

## Process
The process started with obtaining bike stations in Quebec City from the CityBikes API, followed by the park's information available from both Foursquare and Yelp via their respective APIs.
Afterwards, I extracted the total number of parks within a certain radius of a specific bike station and joined that data into a single dataframe, which I then wrote into SQLite3 as a database and database table.
Afterwards, I made some basic graphs with the matplotlib package available in python just to get some sort of sense of what I would get in the statistical model, before running a multiple linear regression model, based on the total amount of bikes at a station and the amount of available bikes at a station for an instance, and compared both to the total amount of parks within the radius of a selected bike station.


## Results
The results led me to conclude that I did not have a strong model. Even just based on the graphs, it was easy to see that there wasn’t really a strong relation between the variables. The results of the model also confirmed that the correlation was weak.

## Challenges 
The challenges for me were about digging through nested json files. It felt like there might have been some information that was buried in the json files, that would have been a bit more difficult to extract and use.
I also had trouble figuring out how to join dataframes, as the Yelp and Foursquare APIs both returned dataframes within a list. I ended up just extracting the desired information and appending it to my main dataframe and only using that single one for the rest of the project.

## Future Goals
If given more time, I would have liked to spend more time exploring the json files, especially the nested information and see if I would have been able to find any interesting data and to extract it. I would also want to be able to have more than a single dataframe, albeit they would all be streamlined and easy to join information onto each other, especially for SQL purposes. Also, with more variety of data, I would have really liked to explore the plotting packages and to make prettier and more presentable graphs.
