# Trend of number of Rides
## by Manju Saini


## Dataset

> The dataset was choosen from list of Udacity provided datasets. The data for each month of 2014 was downloaded from https://www.citibikenyc.com/system-data and than merged into one dataframe, the resulting dataframe was too big for processing, so a random sample of 10000 records was selected and analysis was performed on this small dataset. 

> Data cleanup involved following steps : 
>> removing records where any of the values for 'start station id','end station id', 'bikeid','start station name', 'end station name', 'usertype' was not available
>> converting 'starttime', 'stoptime' to datetime columns, converting 'start station id', 'end station id', 'bikeid' to categorical columns
>> creating columns 'starttime_hour', 'starttime_day_name','starttime_month_name', 'starttime_date' from 'starttime' feature
>> converting 'starttime_hour', 'starttime_day_name','starttime_month_name' to Categorical columns, 
>> creating feature 'tripduration_min' from 'tripduration'

## Summary of Findings

> Most of the trips are made in weekdays(Monday-Friday), this can be because of these days are working days
> Months from May to October have the most rides, with Feburary being the lowest.This can be attributed to temperature being lowest in February.
> More number of rides were observed between 8 - 10 hours, 15 - 20 hours and small peak at 12 hours. People are riding to office, for lunch and back to home.
> 90.3% of the rides are taken by Subscribers and only 9.7% by Customers.
> Top 10 Stations with maximum traffic are - '8 Ave & W 31 St', 'Lafayette St & E 8 St', 'E 17 St & Broadway','West St & Chambers St', 'University Pl & E 14 St','Broadway & E 14 St', 'Broadway & E 22 St', 'W 21 St & 6 Ave', 'Christopher St & Greenwich St', 'Broadway & W 24 St'
> Top 10 Stations with least traffic are - 'Railroad Ave & Kay Ave', 'Church St & Leonard St', 'Sands St & Navy St', 'Macon St & Nostrand Ave', 'Sands St & Gold St', 'Hanover Pl & Livingston St', 'Pershing Square S', 'Avenue D & E 12 St', 'Monroe St & Classon Ave', 'E 33 St & 2 Ave'
> Day of week - rides by Subscribers reduce on weekends(Saturday and Sunday), however rides for Customer increases on weekends(Saturday and Sunday) but still rides by Subsciber on weekends is greater than by Customer.
> Subscribers have a wider range of trip duration but Customers generally have a higher trip duration. 
> More number of short trips are taken on weekdays, and more number of long trips are taken on Weekends
> On Friday evenings's less rides are taken as compared to other weekday's. People are probably travelling to places other than their regular routine, using other modes of transport. On Saturday Subscribers have almost a uniform distribution between 8 hours to 21 hours, but on Sunday there are some spikes at 10, 12, 15, 17 hours, giving us an intution that people may be travelling for some extracurricular classes/activities.
> For Customer type of users, rides during week days are very less, and looks like they ride on need basis. On weekends the number of rides is comparatively greater with peak at 14 hours.
> For Subscriber, total Trip duration in weekdays is mostly greater than that in weekends.While for Customer, Total Trip duration in weekdays is mostly less than that in weekends
> Subscriber - Trip duration and count of rides are greater for months April to October and Monday to Friday. In July, Trip duration and count of trips is maximum on Tuesday, Wednesday and Thursday, giving a intuition that these days might be holidays. Similar but less prominent trend is observed for January-Monday, Thursday, May-Wednesday, Thursday and Friday, August-Thursday, Friday, Saturday, September-Monday Tuesday, Wednesday, October-Friday, April-Thursday
> Customer - Interestingly for June and August - Saturday, Sunday, high trip duration and trip counts observed. Similar but less prominent trend is observed for September-Monday, May-Monday.
> For Subscribers, Total Number of rides decrease in June, then increase again in July.For Customers, Total Number of rides decrease in July, then increase again in August.
> Interaction between tripduration and count of trips gives us an interesting insight about some special days of the year when both the tripduration and count of trips were at high end. Such days can be some holidays or some bike riding event.

## Key Insights for Presentation

> For the presentation, I focused on Trend for Rides and some findings from the analysis. 

> I started by introducing number of rides trend on hourly, weekly and monthly basis, followed by analysing the distribution of tripduration and proportion of rides by each usertype.  I then included the Top 10 high traffic and low traffic stations as this is an interesting point. I then introduced the effect of usertype on number of rides by hour, week, month and tripduration. The interaction between tripduration, number of rides , month, day and usertype was then explained using a heatmap. At last an overall trend was displayed using pointplot.
