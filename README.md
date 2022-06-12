# surfs_up
## Overview of the analysis:
### Purpose of this analysis
In order to determine if the surf and ice cream shop business is sustainable year-round, specifically, in this module and Challenge, we apply Jupyter ```Notebook```, ```SQLite```, ```SQLAlchemy``` and ```Flask App``` to anaylze and present climate data and results. W.Avy would also like temperature data for the months of June and December in Oahu to see the surf and ice cream business can operate as seasonal business.

## Results:
### 1. Using Python, Pandas functions and methods, and SQLAlchemy, first of all, filter the date column of the Measurements table in the ```hawaii.sqlite``` database to retrieve all the temperatures for the month of June and December.
  - Use SQLAlchemy ```extract``` function to get the all **June** dates and temperatures as tuple per row/element
![image](https://user-images.githubusercontent.com/103073631/173224773-95110bab-1db7-4b37-8377-595e213c7fea.png)

  - Use SQLAlchemy ```extract``` function to get the all **December** dates and temperatures as tuple per row/element
![image](https://user-images.githubusercontent.com/103073631/173225162-5f1dff66-e3e8-427b-bd1c-208516550963.png)


### 2. Then convert those temperatures to a list, create a DataFrame from the list
  - create **June** dataframe from the list
![image](https://user-images.githubusercontent.com/103073631/173225216-2eb8e599-71b8-4b97-b395-8bc551408118.png)

  - create **December** dataframe from the list
![image](https://user-images.githubusercontent.com/103073631/173225250-2f90af2e-66c5-4b6d-ab54-f424e992db81.png)

### 3. Lastly, generate the summary statistics.
![image](https://user-images.githubusercontent.com/103073631/173225306-bb4780cc-2d84-4ed5-8bb5-bb19ecb13a4f.png)
![image](https://user-images.githubusercontent.com/103073631/173225322-bb054462-6979-40cb-bac0-c1c0c4c425d2.png)

### Three major points:
1. The mean temperature of 75°F for June is higher than the mean temperature of 71°F for December
2. The standard deviation for June is smaller than December, which means the temperatures in June data are more clustered around the mean.
3. The December temperatures range : max - min = ```83 - 56 = 27``` is larger range than June ```85 - 64 = 21```

## Summary:
From above statistics, we would summize that the temperatures data in June is more normal distributed with recorded temperatures data. The average recorded temperature in June is about 75 degrees F, 4 degrees higher than the average temp in December. By ONLY use the temperatures data for month of June and December, the statistics are reasonably close to each other, it is hard to get the final suggestion if surf aand ice cream shop business can operate year-round or seasonal. We would like to perform additional queries to see if any other factors we need to consider.
- Additional Query 1: June Precipitation and Temperatures, then use matplot and add trendline to see any relations
- Additional Query 2: December Precipitation and Temperatures, then use matplot and add trendline to see any relations
- Additional Query 3: Similarly, to retrieve all the Precipitations for the month of June and December, then covert to list, generate the summary satistics of Precipitation.
- Additional Query 4: run the Stations and temperatures for month of June and December and merge data, to see each station temperatures in June and December
