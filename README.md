# Ride-Share Analysis

Visualizing the analysis of ride-sharing data, consisting of thousands of journeys across hundreds of cities

## Overview of Project

This project consists of an exploratory analysis of large amounts of ride-sharing data, utilizing a range of vizualization types to produce insights from the information. The aim is to illustrate the relationship between the type of city and number of drivers and riders, and the percentage of total fares, riders and drivers by type of city. By summarizing the ride-sharing data by city type, the weekly fares for each city type are then analyzed and displayed using a combination of Pandas and Matplotlib. Deliverables:

- Ride-sharing summary by city type
- Total fares for each city type

### Purpose

The results from the analysis should help to improve access to rideshare services and determine afforability for under-served areas. 

## Data Preparation and Initial Tasks

The software used for this project was Python 3.7.9 and Jupyter Notebook 6.1.4. Before starting the analysis, data was imported from two .csv files for [ride data]() and [city data]() respectively. Below is a summary of the initial analyses performed that can be (found [here]()):

- Imported and inspected the data for completeness
- Sorted data by city type
- Calculated the number of rides, average fare, and average number of drivers for each 'type' of city
- Calculated summary statistics for the above
- Calculated the percentage of total fares, total rides, and total drivers for each 'type' of city

## Results of ride-share data analysis by type of city

In the overall summary of urban, suburban, and rural 'type' cities, it can be demonstrated that:

* In general urban cities have the greatest number of total rides, followed by suburban, then rural
* In general the average fare is highest in rural cities, followed by suburban, then urban with the cheapest
* In general urban cities have a the greatest number of drivers operating, followed by suburban cities, then rural

![]()

Figure 1. Bubble chart summarizing the ride-sharing data by urban, suburban, and rural city types

Looking specifically at the total ride count data, it can be seen that the number of rides are greatest for urban cities, however the range in total rides for these cities varies more greatly and there is one outlier at the upper end. Rural cities which have the fewest number of rides are also show a lesser degree of variability between cities. 

![]()

Figure 2. Total ride count data for urban, suburban, and rural city types

By analyzing at the average fare data for each city 'type' it can be seen that urban cities have the lowest fares on average and rural the highest. However the spread in the data shows that there are a wide range in average fare for all three city types, with rural cities showing the greatest range. 

![]()

Figure 3. Fare data for urban, suburban, and rural city types

Examing the percentage of total fares by city type illustrates the disparity between the three; with urban cities accounting for a whopping 62.7% of overall fares, compared to 30.5% for suburban cities, and 6.8% for rural cities. The higher percentage of total fares collected in urban cities could be due to a larger number of total rides and/or differences in average fare cost.

![]()

Figure 4. Pie chart showing the percentage total fares by city type

Similarly, when the percentage of total rides by city type is vizualized, it can be observed that urban cities also make the most significant number of rides taken with 68.4%, compared to 26.3% suburban, and 5.3% for rural cities, which likely accounts for the higher share of fares. The signficantly larger number of total rides taken would likely explain why the total share of fares collected is also highest for urban cities and these proportions are similar.

![]()

Figure 5. Pie chart showing the percentage total rides by city type

Plotting the percentage of drivers operating in each city type again shows a significantly larger number of drivers operating in the urban cities with 80.9% of the total and just 16.5% in suburban and 2.6% in rural cities in comparison. The larger number of drivers in urban cities may suggest a higher demand for drivers compared to suburban and rural cities, and certainly the higher share of rides and fares in turn supports this notion. 

![]()

Figure 6. Pie chart showing the percentage of total drivers by city type

However, we do not know whether the larger number of drivers in urban cities compared to suburban and rural is solely a result of higher demand, one factor regarding the lower numbers of drivers in suburban and rural cities could also be due to an issue with the lack of supply of available drivers, resulting in less rides taken, and less fares collected. The higher cost of fares in rural and suburban cities might support this idea of supply < demand compared to urban cities. There are a lower percetage of drivers in rural and suburban cities compared to their percentages of total rides and fares. In summary, while there is likely a significantly greater demand for ride-share services in urban cities; suburban and rural cities may be slightly underserved in regards to ride-share availability. 

## Summary of analysis for weekly fare data by city type

Once the statistics were defined by city type, the challenge was to form a summary of those statistics and then create a line graph that shows the total weekly fares for each city type over a period of four months in 2019. The analysis performed for this assignment can be found in [PyBer_Challenge.ipynb](). 

The multi-line chart for total fares by city type over the period of January to April 2019 supports the previous analysis. It can be seen that the fares in urban cities remain the highest throughout all four months, followed by suburban, then rural with consistently the lowest total fares. We can see that fares are lowest at the beginning of the year in january and for urban and suburban cities, then generally rise during the month before fluctuating for the remaining three months. While urban fares remain higher for the remaining three months through february to april, albeit with some fluctuations, suburban cities decrease again somewhat towards the end of january, with larger scale fluctuations in late february and in april. Rural cities generally remain low with comparatively little change throughout this four month period. It is interesting to note that while fares are not always increaseing or decreasing at the same time, all three types of city see a fare increase and major peak during a period in late February, suggesting a common event is likely influencing demand. It is also not clear what is causing the rapid fare increase in suburban cities during april when fares are generally decreasing for urban and rural cities during this period.

![]()

Figure 7. Multi-line chart showing total fares by city type

## Recommendations

As a result of the analyses performed three business recommendations can be delivered to help improve disparities in ride-share services:

* High costs of rides in rural (and suburban) cities could be disuading people from using the services, finding ways to either subsidize the high cost of fares could encourage more riders to use the services in those cities
* Similarly, part of the reason for the high fares is likely lack of available drivers to serve rural and suburban cities, increasing driver pay or creating incentives to attract more drivers to operate in those cities could help improve availability and lower fares
* More data needs to be analyzed to help better distinguish the trends in supply and demand between the city types to find the causes. Other data such as length and duration of rides is not available and may also be a factor in the lower rides, fares, and drivers willing to operate for example. 
