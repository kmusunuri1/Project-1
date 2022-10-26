# Pandemic Preparedness
A pandemic is an epidemic of an infectious disease or virus that has spread across a large region affecting a substantial number of individuals. The most relevant pandemic in recent years is the COVID-19 pandemic that has inflicted turmoil and devastation across multiple continents and continues to evolve into multiple, more aggressive strains of the initial virus. This virus evolution is arguably due to a lack of preparedness and lack of outbreak infrastructure; in our exploratory data analysis project we will investigate the relationship between elements of preparedness: declaration of emergency, vaccination rate, social restrictions, and vaccination accessibility and COVID-19 deaths and hospitalizations.


![covid-19_coronavirus_network_of_vectors_by_da-kuk_gettyimages-1213355637_2400x1600-100837132-large](https://user-images.githubusercontent.com/110564772/197648602-cee38ce3-8e97-4d2d-bf81-42914689c525.jpg)

Essentially, we want to answer the question: what factors indicate an adequate level of preparedness to handle a pandemic? 

To answer this question, we need to evaluate four supplemental questions:

How does vaccination administration impact the rate or volume of COVID cases?

How does government response affect the volume of COVID-19 cases? 

How does vaccine accessibility impact the volume of COVID cases? 

How does a population’s region influence COVID cases?


# Shelter_in_Place.CSV (Merged Table for Analysis)
## Schema
## Name / Type / Description / Example
Date / datetime64 / Each Day from March 2020-March 2021 representing either a date the CDC tracked cases or death or a date that google track Stay at home policy / YYYY-MM-DD 

State / string / identifier for either New York or Texas / NY

Total Cases / int64 / cumulative total of reported cases / 12

Confirmed New C19 Case / int64 / number of new covid cases reported that day/ 12

Total Death / int64 / cumulative total of reported deaths / 12

Confirmed New C19 Death / int64 / number of new covid deahs reported that day / 12

Stay at Home Orders / float64 / number 0 - 3 represnting the policy measures enacted / 0

Stay at Home Orders Codebook:
0 - no measures
1 - recommend not leaving house
2 - require not leaving house with exceptions for daily exercise, grocery shopping, and 'essential' trips
3 - require not leaving house with minimal exceptions (eg allowed to leave once a week, or only one person can leave at a time, etc)
Blank - no data 



Collaborators: Adesuwa Ogiamen, Krishna Musunuri, Kokila Janarthanan, Nasra Ahmed, & Kyndall Butler

