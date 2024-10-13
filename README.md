<div align="center">
    <h1>Citi Bike Trends</h1>
</div>


<div align="center">
    <h4>By: Tai Reagan</h4>
</div>

<div align="center">
    <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/citi-bike-station-bikes.jpg" alt="citi_bikes" width="600"/>
</div>

---

# Project Overview
This analysis examines key Citi Bike trends over the course of one year, from January 2023 to January 2024, to identify significant changes in bike usage across the city. By delving into the most popular start and end stations, top stations overall, average ride durations, and peak ride days and hours, the analysis provides insights into how ridership patterns have evolved. The goal is to provide city officials and public administrators with a clearer understanding of these trends, helping inform decisions related to bike-sharing infrastructure, transportation planning, and urban mobility improvements.

# Link to Tableau Sotry:
[Click to View Tableau Story](https://public.tableau.com/app/profile/tai.reagan/viz/CitiBikeData_17282622527760/Story1?publish=yes)

---

# Itnitial Process: Cleaning The Data
To be able to properly use the data downloaded from [Citi Bikes NYC](https://citibikenyc.com/system-data) the data must be converted to proper formatting so that the data can be used to create visualization in Tableau. The first step is to read in the CSV files into a pandas dataframe in Jupyter Notebook and converting started_at and ended_at into datetime format type. In addition reformatting rideable_type, start_station_id, end_station_id, and member_casual from "object" type to "category' type for both years.


<div align="center">
    <h2>January 2023</h3>
</div>
<div align="center">
    <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/data%20clean%2023.png" alt="23_data_clean" width="600"/>
</div>

<div align="center">
    <h2>January 2024</h3>
</div>
<div align="center">
    <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/data%20clean%2024.png" alt="24_data_clean" width="600"/>
</div>

# Data Visualization 

<div align="center">
    <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/start%20station%20map.png" alt="start_station_map" width="600"/>
</div>

- The first chart provides a geographical map of all the bike rides from their starting station in January for 2023 and 2024. In January 2023, start stations were more densely clustered in central Jersey City, particularly around Journal Square, Downtown Jersey City, and Newport, indicating high bike-sharing activity. In comparison, January 2024 saw a decrease in overall station density and a more dispersed distribution across these regions. Despite this, the Hoboken area consistently showed strong activity, with a slight increase in station density in 2024. The drop in total start stations from 2023 to 2024 may reflect reduced ridership, fewer station activations, or seasonal trends affecting bike usage, particularly in central Jersey City.



---

<div align="center">
    <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/end%20stattion%20map.png" alt="end_station_map" width="600"/>
</div>

- While the second geographical map shows all the bike rides of the ending station in January for 2023 to 2024. In January 2023, the end stations show a high density concentrated around New York City, particularly near the west side of Manhattan and parts of Jersey City, with a maximum count of 2,436. This indicates a significant amount of bike activity terminating in these areas. In January 2024, the overall density of end stations has decreased, with a maximum count of 1,471, suggesting a reduction in total bike trips ending at these stations. However, the distribution remains similar across both years, with a strong focus around Manhattan and Jersey City. The lower density in 2024 might point to fewer bike trips, a shift in ridership patterns, or external factors impacting usage during that period.



---


<div align="center">
  <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/ride%20type%2023.png" alt="23_ride_type" width="400"/>
  <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/ride%20type%2024.png" alt="24_ride_type" width="400"/>
</div>

- A closer examination of the most popular start stations provides valuable insights into Citi Bike traffic patterns, allowing for a deeper understanding of station activity and the types of bikes preferred at different points of departure. Between January 2023 and January 2024, bike usage at key start stations experienced a significant decline. For example, Hoboken Terminal - River St & Hudson Pl, which led in 2023 with 1,796 trips, saw a sharp reduction to just 713 trips in 2024. Other high-traffic stations, such as Grove St PATH, mirrored this downward trend. Interestingly, less prominent stations like 14 St Ferry and South Waterfront Walkway experienced increased activity in 2024, signaling a possible shift in rider preferences or adjustments in bike-sharing infrastructure. The more even distribution of bike usage across stations in 2024 suggests changing travel behaviors and the influence of external factors, potentially related to commuter patterns, infrastructure developments, or broader urban mobility trends. These shifts highlight the need for ongoing monitoring to adapt transportation strategies to emerging user demands.


---


<div align="center">
  <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/avg%20duration%2023.png" alt="23_avg_duration" width="400"/>
  <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/avg%20duration%2024.png" alt="24_avg_duration" width="400"/>
</div>

- The line graph above illustrates the average bike ride duration segmented by member type, offering a clear comparison between casual riders and members in January 2023 and January 2024. Across both years, casual riders consistently exhibit longer ride durations, typically ranging from 15 to 30 minutes, while members maintain shorter, more predictable ride times, largely under 10 minutes. In 2023, casual ride durations display significant variability, with frequent peaks suggesting irregular and extended trips. However, by 2024, casual riders demonstrate a noticeable shift toward shorter, more stable ride durations, potentially indicating a change in behavior or usage patterns. In contrast, member ride times remain relatively consistent across both years, with only slight increases observed in January 2024, underscoring the stable and routine nature of member bike usage. These trends highlight the evolving behaviors of casual riders while reinforcing the steady patterns of members, offering insights into how different user groups interact with the bike-sharing system over time.



---


<div align="center">
  <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/peak%20hours%2023.png" alt="23_peak_hours" width="400"/>
  <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/peak%20days%2023.png" alt="23_peak_days" width="400"/>
</div>

- Examining the peak hours and days for January 2023 and 2024 provides a clearer picture of Citi Bike usage patterns, particularly in relation to commuting and recreational activities. In January 2023, the data reveals two prominent spikes in ride activity, with a significant rise during the morning commute around 8 a.m., followed by a more substantial peak in the late afternoon around 5 p.m. This pattern aligns with typical commuting behaviors. Outside of these hours, ride activity tapers off significantly, with very low usage in the early morning and late evening. The peak days graph for 2023 shows fairly consistent daily usage, with modest fluctuations but no extreme variations, suggesting steady ridership throughout the month.


---

<div align="center">
  <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/peak%20hours%2024.png" alt="24_peak_hours" width="400"/>
  <img src="https://github.com/Taireagan/Citi-Bike-Trends/blob/main/Images/peak%20days%2024.png" alt="24_peak_days" width="400"/>
</div>


- By contrast, January 2024 also shows two distinct peaks during commuting hours, with the highest activity occurring between 7-9 a.m. and 4-6 p.m., further emphasizing that Citi Bike usage is largely driven by work or school commutes. However, there is a more pronounced midday drop in rides, indicating reduced activity outside these key periods. Additionally, weekends, particularly Saturdays, show elevated ride counts compared to weekdays, suggesting a rise in recreational use on non-workdays. The shift in weekend activity points to evolving rider preferences, as more users take advantage of bike-sharing for leisure in addition to commuting. These insights offer valuable context for understanding the shifting dynamics of Citi Bike usage across different times and days.


# Summary
In conclusion there are several key insights from this analysis:
- Commuting Drives Peak Usage:
    - Both January 2023 and January 2024 data show clear peaks in Citi Bike usage during traditional commuting hours (7-9 AM and 4-6 PM).
    - The majority of ridership is tied to work or school commutes.
    - Ride activity tapers off significantly outside these times, particularly during midday and late evening.

- Shift in Weekend and Casual Rider Behavior:
    - In January 2024, there was a noticeable increase in weekend bike usage, especially on Saturdays, suggesting a growing trend of recreational riding.
    - Casual riders in 2024 demonstrated shorter and more stable ride durations compared to 2023, indicating a shift toward quicker, more consistent trips.
 
- Decline at Major Start Stations with Redistribution:
    - Major start stations such as Hoboken Terminal - River St & Hudson Pl saw a significant decline in usage between 2023 and 2024, while less prominent stations experienced increased activity.
    - This shift reflects evolving rider preferences or changes in bike-sharing infrastructure, leading to a more even distribution of bike usage across the network.


Overall, this analysis provides valuable insights into Citi Bike usage patterns, highlighting key trends in ridership frequency, peak times, and shifts in station activity. By identifying high-traffic locations and understanding changes in commuting and recreational use, city officials and public administrators can make informed decisions about where to allocate additional bikes and infrastructure. These insights will help optimize bike availability, enhance transportation planning, and support urban mobility improvements to better meet the evolving needs of riders.





























