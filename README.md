# Data Visualizations with Tableau

View dashboards and storyboard here: https://public.tableau.com/views/Module8Challenge-CitiBikeAnalysisv5/CohortBasedObservations?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

The abiity to determine what data tells the story and how to visualize that story is key to data analytics.  

For this project, the students used Tableau as the data visualization tool. The following is a list of key questions to consider when preparing the workbook:  

-How many trips have been recorded in total during the chosen period?  
-By what percentage has total ridership grown?  
-How have the proportions of short-term customers and annual subscribers changed?  
-What are the peak hours when bikes are used during the summer months?  
-What are the peak hours when bikes are used during the winter months?  
-Today, what are the top 10 stations in the city for starting a journey? Based on data, why do you hypothesize these are the top locations?  
-Today, what are the top 10 stations in the city for ending a journey? Based on data, why?  
-Today, what are the bottom 10 stations in the city for starting a journey? Based on data, why?  
-Today, what are the bottom 10 stations in the city for ending a journey? Based on data, why?  
-How does the average trip duration change by the type of user? (This may be under "User Type" or "member_casual" depending on the period the data is from).  
-What is the average distance in miles for a bike trip?  
-Which bikes (by ID) are most likely due for repair or inspection in the timespan?  
-How variable is the utilization by bike ID?  

# Data download  
I chose to use data from June of each year, 2013-2020, to analyze year over year trends from the beginning of the program. I felt this out give insight about what worked, what didn’t, how the program has grown in popularity, and potential areas for increased revenue. The data is through 2020 because the more recent data does not include some of the attributes I wanted to explore such as age, gender, and year of birth.  

# Data cleanup  
-Imported all files into Tableau and used the union function to combine them into a single source.  
-Renamed the titles to make them more standardized (Bike ID vs bikeid, etc).  
-Used the split function to separate the year and month from the table name column.  
-Grouped the birth years into 10 year cohorts.  
-Created day of week, hour, and year dimensions.  
-Converted bike ID, end station ID, start station ID, birth year, and gendernum from measure to dimensions.  

# Calculations:  
-Number of minutes per trip as the seconds in the trip duration column multiplied by 60.  
-Used an if/then calculation to create a gender column as male/female/unknown instead of numbers.  
-Average trip duration as number of minutes divided by number of trips.  

# Cohort Based Observations Dashboard  
-The bar chart shows that the majority of the users through the time period analyzed were born in the 1970s, 1980s, and 1990s. The box and whisker chart shows these cohorts in the upper hinge and upper whisker, confirming the data.  

-The 2000 cohort has very few trips overall, which makes sense because they were too young to take full advantage of the bikes during the 2013-2020 time frame. The interesting thing is that for all 3 gender designations, the 2000 cohort has the highest average duration as seen in the highlight table. Were they using the bikes for commute vs recreation? Again the box and whisker chart confirms with the purple marker for the 2000 cohort at the very top of each data range.  

-One other interesting phenomenon that the box and whisker chart shows - for those identifying as either male or female, the average number of minutes per trip is tightly clustered range on either side of 20 min so while the number of trips varies per cohort, the length of those trips has less difference.  

# Station Maps Dashboard  
-The animation is a neat way to watch the number of stations increase over the time period as the service area moves both north and east. It also shows how the number of trips has increased year of year as indicated by the increase in size and depth of color.  

# Storyboard Analysis
The storyboard was written as a presentation for a meeting of the Citi Bike stakeholders. It presents the data analysis in the framework of potential areas that can be explored to increase overall bike usage and stakeholder revenue. Suggested areas highlighted:  

-The usage dropped in June of 2020 yet the trip duration increased substantially over the 2019 average. More in depth analysis for cause of this change could show a change in user profile and reveal areas that can be promoted in new marketing materials.  

-Customers vs subscribers shows the beginning of a change from subscribers dominating to a more even split with non-subscribers. What are the best ways to convert those occasional riders to subscribers?  

-The station maps show an expansion of coverage area from 2013-2020. Further research to determine potential markets beyond the current coverage area could lead to increased revenue by moving into new, and potentially underserved markets.  

-Noted differences in usage between the genders reveals a potential to increase revenue through increasing usage by those identifying as female. Further research is needed to find the cause for their lower trip    
