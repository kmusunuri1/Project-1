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


# VAX_RATES.CSV (Merged Table for Analysis)
## Schema
## Name / Type / Description / Example

Date /  datetime64 / Each Day from March 2020-March 2021 representing either a date the CDC tracked cases or death or a date that google tracked vaccination rates / YYYY-MM-DD 

State / string / identifier for either New York or Texas / NY

Total Cases / int64 / cumulative total of reported cases / 12

Confirmed New C19 Case / int64 / number of new covid cases reported that day/ 12

Total Death / int64 / cumulative total of reported deaths / 12

Confirmed New C19 Death / int64 / number of new covid deahs reported that day / 12

New Persons Vaccinated* / float64 / Count of new persons which have received one or more doses / 5988

Cumulative Persons Vaccinated** / float64 / Cumulative sum of persons which have received one or more doses / 356834

New Persons Fully Vaccinated* / float64 / Count of new persons which have received all doses required for maximum immunity / 1546

Cumulative Persons Fully Vaccinated** / float64 / Cumulative sum of persons which have received all doses required for maximum immunity / 164834

New Vaccines Doses Admined* / float64 / Count of new vaccine doses administered to persons / 9542

Cumulative Vaccines Doses Admined** / float64 / Cumulative sum of vaccine doses administered to person / 923449

* Values can be negative, typically indicating a correction or an adjustment in the way they were measured.

** Cumulative count will not always amount to the sum of daily counts, because many authorities make changes to criteria for counting cases, but not always make adjustments to the data. There is also potential missing data. All of that makes the cumulative counts drift away from the sum of all daily counts over time, which is why the cumulative values, if reported, are kept in a separate column.


# VAX_SITES_ACCESS.CSV (Merged Table for Analysis)
## Schema
## Name / Type / Description / Example

Site Name / string / name of vaccination site / Walgreens

Site Latitude / float64 / latitude of vaccination site / 42.9146

Site Longitude / float64 / longitude of vaccition site / 84.3880

State / string / identifier for either New York or Texas / NY

County / string / name of county / Ellis County

Mode of Transport / string / method of transportation / transit

Max Travel Time / int64 / maximum travel time to arrive at site. measured in minutes / 15

Census Pop. 2020 / int64 / estimated population of county in 2020 per census / 19797


# COVID-DEMOGRAPHICS.CSV (Merged Table for Analysis)
## Schema
## Name / Type / Description / Example

CBSA / int64 / Number assigned to US Office of Mgmt and Budget Core-Based Statistical Area / 10580

CBSA Name / string / Name assigned to US Office of Mgmt and Budget Core-Based Statistical Area / McAllen-Edinburg-Mission, TX

State / string / US State Name / New York

% of 25+ Adults Who Completed College 2016-2020 / Float / 26.309091    

Median Age / float / Median age of CBSA / 35.5

2018 Per Capita Personal Income / float / 57,743

2019 Per Capita Personal Income / float / 49,008

2020 Per Capita Personal Income / float / 31,153

Population / int64 / 238691

Total Cases through Oct 2022 / float / 68907.0

Total Deaths through Oct 2022 / float / 652.0

Total Full Vax through Oct 2022 / float / 4544059.0




Collaborators: Adesuwa Ogiamen, Krishna Musunuri, Kokila Janarthanan, Nasra Ahmed, & Kyndall Butler

