---
layout: post
title: "Drunk Driving and Vehicle Theft in Relation to Time"
author: "Xinyi Xu"
# categories: documentation
# tags: [documentation,sample]
image: cuba-1.jpg
---

At the end of March this year, a murder with a gun in Gotha sparked concerns about urban safety in Denmark, so in the case of San Francisco, which is also a big city, we wondered if we could get some insight from the statistical charts on the types of crime and the time of day, as well as the areas where the crime occurs more often than not.

In San Francisco, as in other large cities, crime fluctuates with the rhythm of the city. By analysing historical crime report data from the San Francisco Police Department, we can find some interesting patterns about how criminal activity changes over time. In particular, focusing on specific types of crime that occur on Sundays-vehicle burglaries and DUIs-reveals some unique aspects of city life.

Sunday, for many, is a time of rest and relaxation, a day to gather with family and friends. However, it is also a day that comes with an increase in specific criminal activities, particularly vehicle theft and DUI. Data shows that there is a significant increase in the incidence of these crime types on Sundays, which may reflect the fact that people are more likely to be out and about at the weekend, increasing the chances of vehicle theft. It also seems unsurprising that drink driving offences increase as people attend social events.

In this analysis, we will explore these patterns through three different types of data views: first, a time-series graph showing the distribution of crime events by hour of the day; second, a map view revealing the spatial distribution of crime across San Francisco’s police districts; and finally, an interactive graph allowing users to customise their exploration based on the type of crime or timeframe. Together, these views paint a complex picture of criminal activity in San Francisco, providing insight into the city’s security posture.

## Dataset

<!-- [Getting Started]({{ site.github.url }}{% post_url 2016-10-10-getting-started %}): getting started with installing Millennial, whether you are completely new to using Jekyll, or simply just migrating to a new Jekyll theme. -->
Our dataset is provided by the City and County of San Francisco and owned by OpenData. It includes historical incident reports for the San Francisco Police Department from 2003 to March 2021, and we focus on 2003-2018, with a focus on 7 years of data analysis. The source dataset covers the public safety domain with tags including San Francisco Police Department, crime, police departments, and crime reports. Since its creation in February 2012, the dataset has been viewed over 225,000 times and downloaded over 70,000 times. The dataset is available under an Open Data Commons public domain dedication and licence. Because this journal primarily analyses data on DUI and car theft cases within it, the source link can be found on the San Francisco government’s official website if you need to focus on other crime types.

## 24-Hour Comparison: Sunday Vehicle Theft vs. DUI Crimes

<!-- [Text and Formatting]({{ site.github.url }}{% post_url 2016-09-09-text-formatting %}) -->
The polar graph clearly illustrates the 24-hour cycle of DUI crimes, highlighting a peak occurrence between 9:00 PM and 2:00 AM, with a concentrated peak from 11:00 PM to nearly 1:00 AM. Conversely, the early morning hours from 4:00 AM to 1:00 PM exhibit the lowest frequency of DUI incidents. This pattern is likely influenced by Sunday evening social activities, where gatherings often involve alcohol consumption, leading to decreased vigilance regarding drinking and driving. To mitigate risks, individuals attending such events should consider arranging alternative transportation options to ensure personal safety.

In contrast, the pattern of vehicle thefts throughout Sunday is less immediately discernible. The highest occurrence is observed between 5:00 PM and 7:00 PM, followed by a secondary peak from 7:00 PM to 11:00 PM. Interestingly, incidents between 4:00 PM and 5:00 PM and between 11:00 PM and 12:00 AM are relatively comparable. Notably, the lowest occurrence of vehicle burglaries on Sunday falls between 4:00 AM and 8:00 AM. Taking proactive measures such as securing vehicles in garages and double-checking locks after dinner on Sunday evenings can help reduce the likelihood of theft.

## Sundays: DUI and Vehicle Theft Areas Distribution

<!-- This theme is completely free and open source software. You may use it however you want, as it is distributed under the [MIT License](http://choosealicense.com/licenses/mit/). If you are having any problems, any questions or suggestions, feel free to [tweet at me](https://twitter.com/intent/tweet?text=My%20question%20about%20Millennial;via=paululele), or [file a GitHub issue](https://github.com/lenpaul/Millennial/issues/new). -->

<style>
.container {
  display: flex;
  flex-wrap: wrap;
}

.box {
  flex: 1;
  min-width: 200px;
  padding: 20px;
}

.box iframe {
  width: 100%; 
  height: 200px; 
  border: none; 
}
</style>

<div class="container" style="display:flex; justify-content:space-between;">
    <div class="box">
        <iframe src="./assets/img/fig_vehicle_theft.html" frameborder="0"></iframe>
    </div>
    <div class="box">
        <iframe src="./assets/img/fig_dui.html" frameborder="0"></iframe>
    </div>
</div>

Mission recorded the highest number of DUI cases on Sundays, totaling 186 incidents, whereas the Tenderloin reported the lowest count at 35 cases. Intriguingly, despite its low DUI numbers, the Tenderloin also exhibited the fewest vehicle thefts, suggesting the effectiveness of crime prevention measures, possibly bolstered by stringent police patrols. Various factors such as nightlife vibrancy and law enforcement efforts significantly impact DUI occurrences. For further insights, interested readers are encouraged to consult local law enforcement reports or directly reach out to the LAPD.

Remarkably, the Tenderloin emerges as the safest district on Sundays, tallying only 1566 thefts, while INGLESIDE stands out as the most vulnerable area, with a staggering 2846 thefts. Factors such as population density and parking availability are influential in determining burglary rates.

## Temporal Patterns of DUI and Vehicle Theft Crimes Throughout the Day (2010-2017)

<!-- ![alt text](https://user-images.githubusercontent.com/8409329/32801138-33a72030-c94a-11e7-8a62-6184e6df5a8f.png "Millennial Demo Image") -->
<iframe src="./assets/img/my_bokeh_graph.html" width="100%" height="435" frameborder="0"></iframe>
By analysing the data in a time series, it is possible to observe the pattern of occurrence of drink driving and vehicle theft offences over the course of the day. Drink driving is at its peak from 00:00 to 2:00 a.m., then decreases rapidly until 4:00 p.m. The rate of increase in crimes per hour levels off, and then begins to rise sharply from 6:00 p.m. onwards until late at night. As for the temporal pattern of the occurrence of vehicle theft offences, there are significant differences. Throughout the day, the rate of growth is slower from morning to noon, with a small peak in the midday time period, then suddenly plummeting at 1:00 p.m., followed by a high period of the day until late at night.

Policy recommendations: Based on the analysis of the time patterns, it may be possible to reduce the frequency of both crimes by increasing police patrols late at night, by increasing the enforcement of the law appropriately during the day, by improving traffic management, or by conducting public awareness and education campaigns on weekdays.

### Conclution

<!-- Feel free to check out <a href="https://lenpaul.github.io/Lagrange/" target="_blank">the demo</a>, where you’ll also find instructions on <a href="https://lenpaul.github.io/Lagrange/journal/getting-started.html">how to use install</a> and use the theme. -->
By mapping these crimes to different police districts in San Francisco, we can gain further insight into how certain areas are more likely to be hotspots for vehicle theft and DUI crimes on Sundays. This not only provides valuable safety information for residents and visitors, but also provides data to support law enforcement agencies in developing strategies to deploy resources more effectively, especially on weekends.

In addition, time-series analyses indicate that DUI offences are particularly concentrated during certain hours, which may be correlated with the closing times of bars and restaurants. This finding informs the development of targeted preventive measures, such as increasing patrols during key hours or working with local businesses to promote safe driving awareness.

Overall, through careful data analysis, we are able to not only reveal patterns of criminal activity, but also provide insights into reducing these crimes. By comparing crime data from San Francisco and Copenhagen, we may be able to identify similarities and commonalities in urban crime across different cultural and social contexts. Such cross-city and cross-cultural comparisons may provide valuable insights into global urban governance, prompting urban planners and law enforcement agencies to learn from the experiences of other cities and to work together to improve the safety and quality of life of urban residents.


