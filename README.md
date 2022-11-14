# SLackathon-Weather-Analysis-and-Visualization-Sanas
Ever wondered how the news channels predict weather conditions accurately? It’s because they leverage data science, which is always working in the background in the process of weather prediction. 
## Contents

- [Weather Analysis and Visualization](#submission-or-project-name)
  - [Contents](#contents)
  - [Short description](#short-description)
    - [What's the problem?](#whats-the-problem)
    - [How can technology help?](#how-can-technology-help)
    - [The idea](#the-idea)
  - [The architecture](#the-architecture)
  - [Long description](#long-description)
  - [Conclusion] (#conclusion)
  - [Acknowledgments / Reference Links] (#Acknowledgments / Reference Links)

## Short description

### What's the problem?

Agriculture or farming is the practice of cultivating plants and livestock. Agriculture was the key development in the rise of sedentary human civilization, whereby farming of domesticated species created food surpluses that enabled people to live in cities.Modern agronomy, plant breeding, agrochemicals such as pesticides and fertilizers, and technological developments have sharply increased crop yields, but cause ecological and environmental damage.In agriculture, many times farmers have to spread fertilisers on plants. So before spreading they had to predict weather condition. Is is suitable or not? What will happen in next 1/2 weeks? What is the exact suitable timeperiod? Afer spreding fertilizers they faced lot of challenges like heavy rains washed it all,too much hot weather burns the plant. Due to this at the end, they suffer losses.

### How can technology help?
To help the farmers, they need to predict the weather condition. They need one specific app or tool where they can easily know the weather conditions. And here Data science, Machine learning, Artificial intelligence plays the important role to predict future trend from its historical datas.

### The idea

The idea is like, get the historical weather data and from that data predict the future trend. Analyze it and make it better visualization. 
Rightnow for fertilization, farmers  get the specific timeperiod where it is good to spreadout or wait for somedays or too much risky. They will get the indications that when they can use the ferlizers. 

Future trends- We can see a specific app for farmers where which crops we can grow for that specific time period using weather condition.

## The architecture

![image](https://user-images.githubusercontent.com/80089677/201652007-0b61acbd-6dae-4406-b337-1d5428c17a71.png)

## Long description

# Submission name- Weather data Analysis and Visualization 

Agriculture or farming is the practice of cultivating plants and livestock. Agriculture was the key development in the rise of sedentary human civilization, whereby farming of domesticated species created food surpluses that enabled people to live in cities.Agriculture is one of the sectors most dependent on weather conditions, being its output strongly aﬀectedby them. The eﬀect of abnormal weather conditions on fertilizer application is far from easily predictable. Our focus encompasses both the immediate response to dryness and wetness conditions and, particularly, the lagged response. In fact, from a policy perspective, it is important to understand which are the lasting consequences of these weather phenomena.If a drought or an excess of rain is happening or is foreseen to happen at the time of fertilizer application,the immediate response of a farmer could be to increase the amount of fertilizer to counterbalance the likely output loss caused by the adverse weather conditions or she could opt to reduce it to avoid wasting input expenditures.
The lagged response, as to say the application of fertilizer in a time period subsequent the happening of a weather shock, seems to be more easily predictable. Since a signiﬁcant departure from expected levels of wetness is associated with a reduction in productivity, this implies a lower nutrients up take by plants. This further causes a lower need of fertilization in the subsequent year1. However, although heavy rains may damage cropsas much as drought, they could also cause a run–oﬀ of fertilizer from the soil, thus nullifying this argument.

The project description is organized as follows. Section 1 provides a brief Introduction and describes the data used. In Section 2 we explain the web-scrapping, Pre-processing method, data cleaning. In Section 3 we provide the visualizations and discuss the results. Finally, Section 4 concludes/results


## Section 1- Brief Introduction and describes the data

In this Section we brieﬂy introduce a description of the data used in our analysis. The dependent variable which affects the fertilizer has been taken out. In data"s parameters like temperature, cloud cover, sunshine, global radiation, snow depth, precipitation are being used. 


### Subsection 1.1- Context

The dataset featured below was created by reconciling measurements from requests of individual weather attributes provided by the European Climate Assessment (ECA).

### Subsection 1.2- Content

The list of attributes and their description summaries:

1) date - recorded date of measurement - (int)
2) cloud_cover - cloud cover measurement in oktas - (float)
3) sunshine - sunshine measurement in hours (hrs) - (float)
4) global_radiation - irradiance measurement in Watt per square meter (W/m2) - (float)
5) max_temp - maximum temperature recorded in degrees Celsius (°C) - (float)
6) mean_temp - mean temperature in degrees Celsius (°C) - (float)
7) min_temp - minimum temperature recorded in degrees Celsius (°C) - (float)
8) precipitation - precipitation measurement in millimeters (mm) - (float)
9) pressure - pressure measurement in Pascals (Pa) - (float)
10) snow_depth - snow depth measurement in centimeters (cm) - (float)

### Subsection 1.3- Source

Weather Data - https://www.ecad.eu/dailydata/index.php

## Section 2- Web scrapping and pre-processing

Firstly fetch the required contents form the  https://www.ecad.eu/dailydata/index.php. Data has taken out from 2000 to 2020 years. And data gets pre-processed by several methods. 
Pre-processing Method shown below-
1) Data cleaning- removing unwanted materials.
2) Null values- Filling missing values by manually or by mean or by most probable value.
3) Correcting the features.

## Section 3- Visualization and plots

After completing the pre-processing, performed the several comparisons and plots.

### Subsection 3.1- Cloud cover plots

Cloud cover is an important component of understanding and predicting the weather. Not only does cloud cover impact sky conditions and inform precipitation predictions, it also helps regulate the temperature that occurs in a region.Cloud cover may also influence temperatures at the surface of the planet.The amount of clouds in the sky or the degree of cloud cover. This is one of the main weather parameters, which is also called cloud amount, cloudiness, cloudage, or cloud coverage. 

Today in modern meteorology it is expressed mainly as a percentage. For example, if the sky is 100% covered by clouds, it is a totally cloudy day. If the cloud cover is 25% — the day is more clear than cloudy. The cloud cover of 0% means it is a clear day with no visible clouds at all. So it is also called the percentage of the cloud coverage of the sky.

Cloud cover is one of the parameters which has impact on fertilizer. So to check the cloud cover condition, It gets classified into mostly cloudy, partly cloudy, Obstract view, Barely view. By plotting the graphs, we can easily know that - for a perticulaar day How is the cloud cover status.
Mostly Obstract view means where the cloud cover is more or equal to 9 oktas is riksy period for spreding the fertilizers. Because In obstract view cloud cover indicator '9' indicating that the sky is totally obscured (i.e. hidden from view), usually due to dense fog or heavy snow.

### Subsection 3.2- Snow depth plots

As simple, whereever the snow falls it affects the fertilizer. So it is important to check the snow fall condition. If snow fall shows the 0 means it is good to go ahead for to spread out fertilizers.
Plots shows the mean temp. vs days plot where on which day how's the condition of snow fall. Wheather it is good or it is parshaly good or risky.

### Subsection 3.3- Precipitation level plots

Precipitation include drizzle, rain, sleet, snow, ice pellets, graupel and hail. Precipitation occurs when a portion of the atmosphere becomes saturated with water vapor (reaching 100% relative humidity), so that the water condenses and "precipitates" or falls.
Rainfall intensity is classified according to the rate of precipitation, which depends on the considered time.The following categories are used to classify rainfall intensity:
1) Light rain — when the precipitation rate is < 2.5 mm (0.098 in) per hour
2) Moderate rain — when the precipitation rate is between 2.5 mm (0.098 in) – 7.6 mm (0.30 in) or 10 mm (0.39 in) per hour.
3) Heavy rain — when the precipitation rate is > 7.6 mm (0.30 in) per hour, or between 10 mm (0.39 in) and 50 mm (2.0 in) per hour.
4) Violent rain — when the precipitation rate is > 50 mm (2.0 in) per hour.

So by checking the precipitation level, we can easily known the the rainfall condition. So to checking the rainfall condition we can predict the wheather it is good to go ahaed for spreading fertilizers or not.

Plots shows the on particular day, How much is the precipitation level.

### Subsection 3.4- Temperature effects

Sometimes Higher the temperature cause burn out the crops and also affects on the fertilizers. So the spreding the fertilizers on specific temperature where it is suitable for crops needed.

Plots shows the Temperature level on particular day wheather it is suitable or not.

## Conclusion

Plotting the graphs of cloud cover, temperature effect, precipitation level, snow depth plot we can get to know that when we can spread out the fertilizers.
We can also predict the rainfall, climate condition and take steps accordingly.


## Acknowledgments / Reference Links

1) https://levelup.gitconnected.com/weather-data-analysis-and-visualization-with-pandas-dec9c6078065
2) https://www.researchgate.net/publication/348874159_The_Effect_of_Weather_Conditions_on_Fertilizer_Applications_A_Spatial_Dynamic_Panel_Data_Analysis
3) https://www.researchgate.net/publication/262012705_Variability_of_snow_depth_at_the_plot_scale_Implications_for_mean_depth_estimation_and_sampling_strategies
4) https://www.ecad.eu/dailydata/index.php
