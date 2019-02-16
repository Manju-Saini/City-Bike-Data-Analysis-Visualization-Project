# Trend of number of Rides
## by Manju Saini


## Dataset

> The dataset was choosen from list of Udacity provided datasets. The data for each month of 2014 was downloaded from https://www.citibikenyc.com/system-data and than merged into one dataframe, the resulting dataframe was too big for processing, so a random sample of 10000 records was selected and analysis was performed on this small dataset. 

> Data cleanup involved following steps : 

>> removing records where any of the values for 'start station id','end station id', 'bikeid','start station name', 'end station name', 'usertype' was not available

>> converting 'starttime', 'stoptime' to datetime columns

>> converting 'start station id', 'end station id', 'bikeid' to categorical columns

>> creating columns 'starttime_hour', 'starttime_day_name','starttime_month_name', 'starttime_date' from 'starttime' feature

>> converting 'starttime_hour', 'starttime_day_name','starttime_month_name' to Categorical columns, 

>> creating feature 'tripduration_min' from 'tripduration'

## Summary of Findings

> In the exploration, I found Subscriber usertype are riding more on weekdays than weekends, probably for travelling to/from office/schools. However, Customer usertype mostly ride during weekends. It was interesting to find that 90.3% of the rides are taken by Subscribers and only 9.7% by Customers. 

> If we look at tripduration for Subscribers and Customer, Subscribers have a wider range of trip duration but Customers generally have a higher trip duration.

> Top 10 Stations with maximum traffic were found to be - '8 Ave & W 31 St', 'Lafayette St & E 8 St', 'E 17 St & Broadway','West St & Chambers St', 'University Pl & E 14 St','Broadway & E 14 St', 'Broadway & E 22 St', 'W 21 St & 6 Ave', 'Christopher St & Greenwich St', 'Broadway & W 24 St'

> Top 10 Stations with least traffic were found to be - 'Railroad Ave & Kay Ave', 'Church St & Leonard St', 'Sands St & Navy St', 'Macon St & Nostrand Ave', 'Sands St & Gold St', 'Hanover Pl & Livingston St', 'Pershing Square S', 'Avenue D & E 12 St', 'Monroe St & Classon Ave', 'E 33 St & 2 Ave'. More analysis regarding these stations can be done to improve traffic and thus turnover from these stations.

> Analysing the weekly trend, it was observed that on Friday evenings's less rides are taken as compared to other weekday's. People are probably travelling to places other than their regular routine, using other modes of transport. And on Sunday's,  there are some spikes at 10, 12, 15, 17 hours, giving us an intution that people may be travelling for some extracurricular classes/activities.

> Interaction between tripduration and count of trips gave us an interesting insight about some special days of the year when both the tripduration and count of trips were at high end. Such days can be some holidays or some bike riding events. More analysis can be done regarding such days which can help the company in improving turnover.

> Overall trend for the year 2014, followed weather cycle with minimum rides during lowest temperature in Feburary and more rides when temperature was pleasant during May to October.

## Key Insights for Presentation

> For the presentation, I focused on Trend for Rides and some findings from the analysis. 

> I started by introducing number of rides trend on hourly, weekly and monthly basis, followed by analysing the distribution of tripduration and proportion of rides by each usertype.  I then included the Top 10 high traffic and low traffic stations as this is an interesting point. I then introduced the effect of usertype on number of rides by hour, week, month and tripduration. The interaction between tripduration, number of rides , month, day and usertype was then explained using a heatmap. At last an overall trend was displayed using pointplot.
