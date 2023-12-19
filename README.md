# TFL 2022 BIKE RIDES REPORT
## Presented by: Ekene Christian Ikeakanam
___

## INTRODUCTION AND PROBLEM STATEMENT
___
The Transport for London (TFL) Cycling Scheme is a public bike-hiring scheme sponsored by Santander and operated by Serco in London, United Kingdom. It forms part of the Mayor of London's Transport Strategy aimed at ensuring eighty percent (80%) of trips in London are done by walking, cycling, or using public transport by the year 2041 to promote safety and healthy living and ease up traffic congestion.

In line with the mayor's long term strategy, This project was embarked upon to investigate the following observations and more:
-  Record of cycling trips for the selected year
- Comparison of the recorded trips to the annual projection
- Most popular or busiest stations and locations
- Identification of cycling patterns during various seasons, months, days and hours
- Duration of cycling trips during the course of the selected year
- Factors that influence and promotes cycling in terms of volume and duration of rides

## Dataset and Source of Data
___
The dataset of bike rides in London is provided by Transport For London (TFL) and openly accessible for research and analytical purposes online at [TFL Bike Ride Dataset](https://cycling.data.tfl.gov.uk/).

The dataset was obtained from multiple csv files each of which contained records of bike rides across various weeks and months over the year 2022. Each csv file contained a single table with multiple columns respectively which includes: Rental ID (Primary Key), Duration, Start and End Date, Duration, Start and End Stations.

## Demonstrated Skills
___

## 1. Preparation of Data

### Import Datasets
The dataset containing multiple csv files were saved in a folder and imported from my computer using the Get Data feature available on Power BI. This was done using the import storage mode as there wouldnt be any need for data refreshes and loaded to the Power Query editor.

### Combine Datasets 
All imported datasets across multiple csv files contained formatted tables with similar structures and as a result of the similarity in structure, they were appended collectively as a new query into a single dataset in the power query editor for further transformation

### Data Transformation: 
A number of data transformation processes was executed on the dataset, some of which includes:
- Identification and removal of unwanted columns to minimize the model size
- Rename columns and update data types as required
- Creation of additional columns: Season (Summer, Winter, Autumn or Spring), Hour of the day (integer values between 0 - 23), Day of the week (Monday - Sunday) all of which were obtained from the Start Date Column, Duration in Minutes amongst others.
- Cleaning of data by dealing with missing / null values, removal of duplicates and ensured only valid records of rides between Jan 1 - Dec, 2022 were added to the model.
- Checked the quality and distribution of data using Column Quality, Profile and Distribution feature in Power Query Editor.
