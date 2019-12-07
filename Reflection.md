# Milestone 2

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


# Milestone 3


## Summary of Peer Review Feedback
We received feedbacks from peers who are not members of our group and they reviewed our interactive dashboard. The key points are summarized below:

- We need to communicate whether the crime counts in the geo map are normalized by population
- Change months from digits to actual month names and change year to a nominal or ordinal data type in crime rate plot.
- Change hour to actual time of day instead of a number.
- Use line and bar chart together can keep consistency
- Add description/titles on top of the region and type of crime drop-downs
- Add description for Crime Rate graph (mention that it is normalized for population)
- Provide users some information about which dropdown controls which graphs so that users know which buttons control which plots.
- In the dropdown box, provide the selection 'all' so that users can add all districts back using only one click.

## TA Feedbacks from Milestone 2
- Add a description of the app at the beginning.
- Fix the range of the color scale with changing neighborhoods and years, as it gives the user the ability to compare between different scenarios.
- Include or cite the data source.

## Action Items
- Change months to actual month names
- Change year to a nominal or ordinal data type in crime rate plot.
- Titles for the filters of "Area" and "Type of crimes"
- Add description for Crime Rate graph (mention that it is normalized for population)
- Another improvement is that in the dropdown box, provide the selection 'all' so that users can add all districts back using only one click.
- Fix the range of the color scale with changing neighborhoods and years, as it gives the user the ability to compare between different scenarios.

## Completed
Changed months from digits to names of months
Changed year to ordinal type in crime rate plot
Cleaned up code to follow tidyverse standard and PEP 8
Added description of dashboard
Titles for the filters of "Area" and "Type of crimes"

## Ongoing Items
- Create Vancouver map in ggplot. The process of creating the map in ggplot is taking longer than anticipated. We will continue working on it.
- Titles for the filters of "Area" and "Type of crimes" (completed in dev branch)
- Cite the data source

## Pending
- Fix the range of the color scale with changing neighborhoods and years, as it gives the user the ability to compare between different scenarios

## Conclusion
As a matter of time constraint and advanced technical complexity of some requirements and feedbacks, we are unable to complete the implementation of all the reviews. However, we will attempt to review some of them on case by case basis and as time permits. 