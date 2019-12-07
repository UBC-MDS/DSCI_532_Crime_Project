# Milestone 2 - Reflection

## Implementation
We have built an interactive app that has the capability of displaying the crime information of Vancouver neighbourhoods, different crimes and years at a glance. This app answers questions regarding general crime trends in Vancouver and creates awareness about crime rates per neighborhood and the necessity for drastic intervention. 

## What did we do?

We obtained data from Vancouver Police Department between 2003 to 2019, but since 2019 data was incomplete, we had to exclude it so that proper comparison between the years can be made. Using an incomplete year will not be a good reflection of year-year comparison information.

## What worked?
The dashboard has five different plot sections: crimes in Vancouver, crime occurrence by month, crime occurrence by time of day, crime rate, and constituents of selected crimes. These various charts helped provide a comprehensive information about the subject, depending on the information sought by the user. Also, we implemented multiple-select option for the plots in the dashboard which ensured many cities, year, and crime types are selected, and we made all variables to be selected by default which gives the initial full picture and the user can fine-tune the selections options for specific information.

We also used the map plot with tooltips for better visualization, and a combination of the plot sections helps answer the research question. The appropriately labeled plots also incorporated good use of color for clarity. Team effort was key, as breaking down the tasks into little chunks and delegating responsibilities made the project a success. 

## Approach
To calculate the crime rate (number of crime occurrences per 1000 people), we needed population data which we obtained from [Government of BC website](https://www2.gov.bc.ca/gov/content/data/statistics/people-population-community/population/population-estimates) and  [Vancouver Census Local Area Profiles data](https://data.vancouver.ca/datacatalogue/censusLocalAreaProfiles2016.htm). These were integrated into our app and original data and used for the analysis.

## Limitations
For crime rate plot, the year is of type quantitative instead of Ordinal. We are aware of this, but changing type to ordinal caused issues to the plot. The issue is the output of line as straight and not expected reflection. The app lists only the crimes that were reported to the police department and may not be the actual number of crimes that happened in Vancouver. We had to exclude crimes like `Homicide`, `Offence Against A Person` because no association with any neighborhood was made. To maintain consistency in the app, we excluded crimes that happened in the city but had no association with any neighborhood.


## Areas of improvement 
We plan to improve the app by making the dropdowns and slider to be by the side bar, and not up. We also will figure out how to use year as ordinal instead of quantitative in the crime rate plot. Another area of improvement will be to generalize this project to the entire area of BC.

## TA Feedback
We have modified our team contract to include the specific role of each team member and modified the app description accordingly to include multi-select option which we implemented.


# Milestone 3 - Reflection


## Compliments of the App
Many of our batchmates appreciated the effort we put in developing this simple app that helps residents & visitors of Vancouver to visually analyze crime data. Without any introduction on how to use the app, many of our peers were able to gain insights on what we desired them to have.

## Summary of Peer Review Feedback
We received feedback from peers who are not members of our group and they reviewed our interactive dashboard. The key points are summarized below:

Issues we improved upon in the new version of the App:  
- Changed months from digits to actual month names.
- Changed year to a nominal data type in crime rate plot.
- Added description/titles on top of drop-downs to provide users some information about which dropdown controls what part of the app.
- Communicated whether the crime counts in the geo map are normalized by population.
- Added a description for Crime Rate graph (mentioned that it is normalized for population).  
- In the newly deployed version of the app we have cleaned up code to follow tidyverse standard and PEP 8 style formatting.  


Issues not addressed:  
- In the dropdown box, provide the selection 'all' so that users can add all districts back using only one click.  
  - We tried including a reset button to reset all the filters but given the time constraint, we could not spend much time on this. But this functionality can be achieved if the user just reloads the page.  
- Change hour to the actual time of day instead of a number.  
  - We thought it's best to keep the time of day in the units of hours because it does convey what we are trying to show and we think there is no easier way for a user to visualize Time of Day as hours of the day.  
- Use line and bar chart together can keep consistency  
  - Line charts effectively show trends like crime rates and effective visualization holds more importance than consistency in the app.  


## TA Feedbacks from Milestone 2
- Add a description of the app at the beginning.
    - Completed in the latest deployment of the app.
- Fix the range of the color scale with changing neighborhoods and years, as it gives the user the ability to compare different scenarios.
    - We understand how this might create confusion for the user whenever he changes the filter. Since this a big development, we will try to incorporate this in the next phase of deployment.
- Include or cite the data source.
    - Link to the data source is provided in the Github repository


## Ongoing Items
- Create the Vancouver map using `ggplot`. The process of creating the map in `ggplot` is taking longer than anticipated. We will continue working on it.
- Working on developing the application from `dashR`
- Fixing the range of the color scale with changing neighborhoods and years, as it gives the user the ability to compare different scenarios

## Conclusion
It was a great exercise to receive & give valuable and constructive feedback to different apps developed by our friends in MDS 2019-20 batch. No matter how much we want to incorporate every feedback we received from our batchmates, given the time constraint and technical complexity of further development, we are unable to complete the implementation of all the reviews. However, we did collate all the feedback and prioritized them based on the relevance of the feedback and the time we had to incorporate them. Going further we will attempt to review some of them on a case by case basis as time permits. 


