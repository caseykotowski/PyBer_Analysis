# PyBer Analysis
### Overview
This analysis takes ride sharing data for many cities across the US, categorized by city type (rural, suburban, or urban). My goal was to take this data and sort fare prices by various variables to discover what might cause fares to change price. I looked at just city type, but to dig a little deeper I looked at the combo of city type with number of rides per city, and number of drivers per city, as well as time of year.

### Results
In general, fare prices are highest in rural cities, and lowest in urban cities (with suburban fares falling in between). 

![Pyber Data DataFrame](https://github.com/caseykotowski/PyBer_Analysis/commit/c1d19349a881f39c049228b44001198c0028fd60)

This DataFrame lays out all the details for ride data by city type. Total rides are inverse to fare costs, with urban cities having the largest total number of rides, and rural cities having the fewest total rides in the timeframe of my data. 

The next column states the total number of drivers. The more rides in a city type, the more drivers there are. There are actual more drivers available than rides taken in urban cities, meaning in the time the data was collected, some urban drivers did not work. 

The next column shows the total fares collected by city type. Despite having the lowest fare per ride, urban cities collected by fare the most fares total. The more rides, the more opportunities to collect fares, more total fares collected. 

Now the DataFrame gets into a bit of analysis. What does the average rider pay per ride in each city type? Rural rides come in with the highest per ride average, and urban rides are on average the least expensive. 

Now the average fare per driver in a city type column is the most interesting to me. With more urban drivers than rides taken, that fare is greatly skewed down. But, with more drivers available, each ride is on average less expensive. 

But is the time of year a factor? To look at this, I sorted the rides by date as well as city type, and regrouped to see the fares collected per week. The below chart shows how fares change over time for the first quarter of 2019. 

![PyBer Fare Summary](https://github.com/caseykotowski/PyBer_Analysis/blob/473e5acc06b328092272e263d52b9ce0b436c1c9/analysis/PyBer_fare_summary.png)

The year started off with lower fares for all city types, with fares peaking around the beginning of February. But each city type took its own trajectory with fare prices over the months plotted. The chart does, however, show that Rural fares are consistently the most expensive, and Urban fares are the least expensive. 

### Summary
Overall, it is much more expensive to take a ride sharing trip in a rural city than an urban city. This could be for a varity of reasons, but might include how many drivers are available, or how many rides are taken in a city. There were many potential variables that were not taken into consideration. If I redid this analysis, I would have included the distance of rides into consideration. From my knowledge of city type make ups, I would guess that the fewer people in a city, the longer an average ride would be. If the ride cost is based on distance, then rural and suburban rides are going to be more expensive.

As for recommendations to the ride sharing company to address the cost disparity, I have three:
* Redistribute some of the out of work urban drivers to the suburban or rural market. Maybe you could add an incentive to taking those types of rides such as a greater percentage of the fare. 
* If the fares are calculated by distance, take the distance divided by a city's population density to reduce fares for rural and suburban cities by taking into account how much further apart destinations are there.
* Offer incentives for rural and suburban riders (maybe extra rewards points or something) to take more rides, so there is more competition to push down prices. 
