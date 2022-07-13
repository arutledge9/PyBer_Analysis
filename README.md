# Pyber with Matplotlib

## Overview

I've been working with my coworker, Omar, at the ridesharing company Pyber to analyze ride data across many cities for our CEO utilizing Pandas DataFrames and the Matplotlib library. This particular assignment entailed creating a summary DataFrame of the ridesharing data by city type - urban, suburban, and rural - and then plotting the data on a multiple-line graph to illustrate the city types' weekly fares across approximately four months so I can provide Pyber with data-driven insights on the differences between the city types to best drive business decisions.

## Results

I began my analysis by digging into the differences between the city types' data as detailed on the summary DataFrame:

![](Resources/summary_df.PNG)

We can see right off the bat that there are large disparities between each city type and their respective total rides, drivers, and fares:
- **Total Rides:** Total suburban rides (625) are five times the total rural rides (125), while total urban rides (1,625) are 2.6 times the total suburban rides - and urban rides are *thirteen* times the total rural rides! 
- **Total Drivers:** At 78 total drivers, our rural cities are 6.3 times less than our suburban drivers (490), which in turn are 4.9 times less than our urban drivers (2,405).  We also have nearly 31 urban drivers for each rural driver. 
- **Total Fares:** Here, our total rural fares ($4,328) are approximately 4.5 times less than our total suburban fares ($19,356), which are roughly 2.1 times less than our total urban fares ($39,854), which, in turn, are 9.2 times more than our total rural fares. 

Our Average Fares per Ride and Driver also illustrate large disparities:
- **per Ride:** A rural rider pays an average of $34.62 per ride, which is about 1.12 times greater than the average fare for a suburban driver ($30.97), which, in turn, is about 1.26 times greater than the average urban fare of $24.53. Accordingly, rural riders pay on average abour 1.41 times more than urban riders. 
- **per Driver:** Given all of these differences, it therefore shouldn't be surprising that we also see different average fares for our drivers. Rural drivers pull an average fare of $55.49, 1.4 times more than their suburban counterparts ($39.50). However, both of these figures dwarf our average urban fare of $16.57 (2.38x less than suburban fares and 3.5x less than rural fares). 

From our summary DataFrame, I moved to our multiple-line graph:

![](Resources/weekly_fare.PNG)

In layman's terms, this graph takes our "Total Fares" column from the summary DataFrame and lays it over the four months we're examining, looking at our fares one week at a time - again, split out by each city type. There are some interesting patterns here where 2 city types may move in tandem - for example, a rise in fares for urban and rural in the second week of January, while rural fares decline (and the inverse for the first week of February) - and some where all three move in unison, most notably the week prior to March, and the week following. Without knowing the specifics of what may be happening locally during these time periods, I find it difficult to draw conclusions based on these "in tandem" fare movements, but they may be worth exploring with additional data. 
