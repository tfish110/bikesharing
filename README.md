# bikesharing
## Overview

The task for this challenge was to utilize August 2019 New York City user data from Citibike as market research to determine the most important factors for expanding Citibike services to Des Moines, Iowa. With this data, I created a number of visualizations using Tableau in order to present the story behind this user data to potential investors. 

### Resources
- Data:
    - Original source: https://s3.amazonaws.com/tripdata/index.html
    - Modified data file: citibike_df_datetime.csv
- Software: Gitbash 2.37.1.windows.1, Python 3.7.13, Conda 4.13.0, Jupyter Notebook 6.4.8, Pandas 1.3.5, Tableau Desktop Public Edition 2022.3.0

## Results

![Landing Dashboard 1](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image1.jpg)
Here is the initial dashboard for the Tableau Story which gives an overview of the number of Citibike rides in the New York City August 2019 dataset, the proportion of subscribers to single-use customers, the gender breakdown of the customers, and a map of the relative frequencies of Citibike trip starting locations.

![Landing Dashboard 2](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image2.jpg)
I utilized Tableau's feature to simply copy the initial dashboard and add text boxes to point out the important features of profiling who the most likely customers might be. Here, I emphasize that subscribers far outnumber single-use customers in the dataset.

![Landing Dashboard 3](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image3.jpg)
Continuing the thought process of developing a typical user profile from the previous copy of the initial dashboard, this new text box emphasizes that about 2/3 of the users are male.

![Starting Locations Map 1](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image4.jpg)
Here, I expanded the starting locations map from the opening dashboard to point out that Midtown Manhattan seems to be the area of most frequent use, and that this particular part of the city is a very popular tourism area.

![Starting Locations Map 2](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image5.jpg)
Again using the duplication and text box features, I repeated the map and highlighted that Lower Manhattan seems to be the second most popular area for Citibike usage, and that there are many office buildings in both this area and Midtown Manhattan, meaning that commuters may also be a good population segment to target.

![Ending Locations Map](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image6.jpg)
Here I provided the ending locations map simply to point out that the starting and ending location maps appear very similar, so unless there are very specific cases for only one-way trips being made, high-usage hot spot areas will need more bikes regardless of whether on an individual basis someone is starting or ending there trip there.

![Hourly Usage Rates](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image7.jpg)
This horizontal bar chart displays the number of rides started at each hour of the day in the dataset. I used Tableau's highlighting/selection feature to emphasize the six most frequent hours of use, and point out the continuation of the story that commuters are a good candidate population to target for expanding to a new city.

![Trip Duration](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image8.jpg)
This line graph shows that the vast majority of rides last less than 20 minutes, and almost zero rides last an hour or more. This is good evidence to emphasize the speed and convenience that the service can provide for navigating a busy city.

![Trip Duration by Gender](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image9.jpg)
This is the same data as the previous graph, but with the user population broken down by gender. While there were many more men using the service than women, gender did not seem to impact the way the service was used: mostly short trips lasting less than 20 minutes, with nearly zero lasting an hour or more.

![Hourly & Weekday Heatmap](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image10.jpg)
This heatmap shows the relationship between the day of the week and hourly frequency of use. Much like the earlier bar chart seemed to correlate strongly with morning and evening rush hour travel times, this heatmap expands on that story even further by showing that those hours are indeed the most popular Monday-Friday. But, on Saturdays and Sundays, Citibike usage seems more evenly spread through the hours of the day rather than concentrated on those two peak timeframes.

![Hourly & Weekday Heatmap by Gender](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image11.jpg)
Similar to the trip duration line graph being broken down by gender, we now have the same hour and weekday heatmap broken down by gender. Much like that trip duration line graph, we can see here that while there is a greater number of male users, the hourly and daily "commuter pattern of use" that we see is still present in the heatmap of female users, but just in less intense colors due to having fewer female users overall compared to males.

![Weekday Heatmap by Gender & Usertype](https://github.com/tfish110/bikesharing/blob/main/Resources/NYC_Citibike_Challenge_image12.jpg)
This heatmap comparison is similar to the last one, but instead of looking at hour, weekday, and gender, here we are looking at subscription status, weekday, and gender. As we know from the previous heatmap, male and female users show the most frequent use on weekdays rather than weekends; however, here we can see that this pattern really only seems to exist in the subscriber subset. This indicates that the peak use of Citibike most surely be commuters, as in addition to our previous evidence of time of day and day of the week, we can now see that subscribers are the ones doing this on a regular basis. The implication is that they are using Citibike as a way to commute on a regular basis, not just when they miss a train, are having trouble hailing a cab, the weather is bad, or some other extenuating circumstance.

## Summary

Overall, it seems that the story told through the Tableau visualizations is clear: commuters are the largest share of users, and when expanding Citibike's services into a new city, they are a great population to target for advertising. There are however hints in the data of some other avenues to explore for expanding the user base. First, if our conclusions throughout the data story are that men and women are using the service in similar ways, why is it that women are a much lower share of the user base? One possible factor could be age; perhaps only younger women are using Citibike, while a broader age-range of men are using it. There is age-related data in the dataset, so this could be a good route to explore further.

Another topic that can be covered is examining the geographic relationship with the times that Citibike is used. As our map visualizations suggested, tourists and commuters could both be good candidates to target for the service, and the visualizations presented here really only tell the story of commuters. Breaking the geographic maps down into weekday vs. weekend maps to track the frequency of use based on location could highlight tourism hotspots, as those would be expected to be busier on weekends, as opposed to commuter hotspots being busier on weekdays.