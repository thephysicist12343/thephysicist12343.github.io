# Forecasting Desert Locust Distribution 
This page is a description of a project I presented at the Regeneron International Science and Engineering Fair (ISEF) with fellow student Abhimanyu Singh, which received a fourth grand award in the Environmental Science category. 

## 1. The Abstract

Desert Locusts/Schistocerca gregaria (Forskål) constitute a serious threat to food security, with the 2020 swarms causing 8.5 billion USD worth of damages in East Africa and Yemen alone. Existing locust-control tools use real-time field data to monitor developing swarms for immediate control operations. However, these tools do not account for long-term climatic and marine influences like the Indian Ocean Dipole (IOD), that significantly impact rainfall and locust migration patterns. 

This study presents LocustTrack, a novel tool that contains both a short-term weather model and a long-term Species Distribution Model (SDM) to predict locust distribution from the present till the year 2100 by assessing whether ecological or climatic conditions are favourable to locust swarm occurrences. The SDM integrates climate, crop and human footprint data, while the weather-model incorporates future precipitation, temperature and wind-circulation data. 

Climatic data in the long-term model is taken for different Socioeconomic Pathways (SSP) scenarios, which represent different possible carbon emission scenarios. LocustTrack also pioneers the use of marine-data layers from Bio-ORACLE and predicted Dipole Mode Index (DMI) values depicting the state of the IOD from the National Aeronautics and Space Administration (NASA) . 

An environmental justice index was created by comparing the number of swarm occurrences to control operations (as recorded by the FAO). This was then plotted on the Quantum Geographic Information System (QGIS), allowing for the identification of areas underserved by locust control efforts. 

The SDM achieved an AUC of 0.983, while the weather-model, presented as a monthly-risk dashboard for farmers till 2099, had an accuracy of 97.4%. 

The SDM predicted a correlation between carbon emissions and locust occurrences, as represented by the SSPs. According to the model, the probability that locusts will exist in areas without any former locust occurrences significantly increases, and the probability of swarm occurrences in areas currently impacted by swarms increases significantly under most emission scenarios. 

LocustTrack is a low-cost tool that offers critical lead time for proactive locust control measures, timely procurement of safe biopesticides from UN and early harvesting of mature crops, thus ensuring food security (UN-SDG-2) for locust-affected areas.

## 2. The Motivation & Background

Locust swarms pose a major threat to agriculture today, with some even considering them the most dangerous extant pest. 1 square kilometre of a locust swarm can have up to 80 million adults and eat the same amount of food as 35,000 people in a day. Swarms are also getting worse, with the devastating 2020 East Africa swarms reaching 2,400 square kilometres and locust breeding seasons shifting due to unseasonal precipitation as a result of climate change.

The economic impact of swarms is monumental, and the The World Food Programme estimates that long-term response and recovery costs top $1 billion per upsurge, not accounting for crop losses due to swarms. However, the human cost is even more tragic: 20.4 million people were faced with food insecurity after the 2019-20 upsurge. To make matters worse, swarms disproportionately impact the least developed nations. 

While locust swarms are natural, they extent to which they are observed in the modern day is not. Studies such as Saha et al. (2021) and Kimathi et al. (2022) have served to show the connection between locust breeding and distribution and rising temperatures. This is elaborated upon in the Section 3. 

This project is associated with the following UN SDGs:
1. SDG 1: No Poverty
2. SDG 2: Zero Hunger
3. SDG 10: Reduced Inequalities
4. SDG 13: Climate Action

## 3. Prior Research & Locust-Tracking Systems

The United Nations’ Food & Agriculture Organisation (FAO) is the main organisation responsible for real-time monitoring of locust swarms across countries, using data from ground survey stations. While the FAO's work is not only commendable but advanced, there is scope for improvement as monitoring is currently restricted to short-time warning and predictions. 

The recent upsurge of 2020 demonstrated this clearly, with locusts entering nations like Kenya, which have not been affected by locust upsurges for 60 years. This was the result of unchecked breeding in East Africa: three generations bred, with each generation multiplying the number of locusts by approximately twenty times, finally leading to a colossal number of locusts. 

Saha et al. (2021) and Kimathi et al. (2020) are studies that have used MaxEnt for predicting locust distribution, a publicly available software that correlates environmental data with presence-only species occurrence data for species distribution modelling. These efforts have paved the way for our work, yet there is still insufficient research on
1. The impact of marine influences on locust distribution
2. How locust distribution is impacted by climate change
3. Robust models that use advanced forms of machine learning to model locust swarms

## 4. Research Questions

To answer our questions and achieve our aim, we explored three broad research questions:
1. Can we accurately model and forecast potential breeding hotspots (young locust nymphs) and the distribution of swarms (adult locusts)?
2. Are changing climatic conditions and novel marine influences (like the IOD) significant contributors to the spread of locusts?
3. Are any geographic areas vulnerable to attacks underserved by current locust control operations, and how can they be identified?

To answer our questions, we created three models: a short-term breeding model to predict locust breeding, a long-term climate model to explore the influence of climate change and marine influences on locust distribution, and an environmental conditions map to explore the inequitable impact of locust swarm-associated damage. 
