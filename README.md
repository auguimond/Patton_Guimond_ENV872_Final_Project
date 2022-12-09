# <Patton_Guimond_ENV872_Final_Project>

## Summary
Our final project focuses on exploring temperature tends at four different U.S. military bases. Four initial data sets were obtained, one for each of the U.S. military bases in the study. Data sets contain several climate variables recorded in hourly intervals between 2012 and 2022. Using this data, we explored if military bases have seen changes in temperature and wet bulb globe temperature that would interfere with future operations based on heat concerns. The data files contain climate data for Forts Jackson, Sill, Leondard Wood, and Benning. Data was analyzed using a combination of time series analysis and graphing to determine if there are significant trends at each location. The repository contains raw files with unedited climate data for each base. It also has edited drafts of the same data files which are better suited for analysis. All draft R markdown files are contained in RMD folder. These files are drafts and versions of time series and other analysis code that went into the final report. All the knitted files and drafts are contained in the knitted folder. The final project markdown file contains the report for the final project for ENV872L Environmental Data Analytics. 

## Investigators
Austin Guimond, Master's Student at Duke's Nicholas School of the Environment, 
Email: austin.guimond@duke.edu

Erik Patton, Doctoral Candidate, Duke University Nicholas School of the Environment
Email: erik.patton@duke.edu

## Keywords
Wet Bulb Globe Temperature
Mann Kendall
Seasonal Mann Kendall
Heat Category
Army Basic Training
Fort Jackson 
Fort Sill
Fort Benning 
Fort Leonard Wood


## Database Information
Temperature files for the four military installations were created by the U.S. Air Force 14th Weather Squadron, stationed in Ashville, NC. Files were requested through a CAC-card enabled support portal.

Ft Jackson data was created on October 13th, 2022 by Senior Airman Rachel Hamelin.

Ft Sill, Ft Benning, and Ft Leonard Wood data was created on November 9th, 2022, by Mr. Jeffrey W. Budai.

Military installation shape files were obtained from the Defense Installation Spatial Data Infrastructure repository. File are available through a CAC-card enabled support portal and accessed on November 28th, 2022.

County and State shapefiles were obtained from the US Census beauru, available at: https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html

## Folder structure, file formats, and naming conventions 
Data- The data folder is subdivided into Geospatial, metadata, processed data, and raw data. The geospatial folder contains all the data used for geospatial analysis. Processed data contains all the files that were altered in some way for analysis including the removal of unnecessary rows. The raw folder contains raw, unedited csv files. 

Final Project Markdown- Contains the RMD file for the final report that satisfies the requirements for the final project in ENV872L. 

Knitted Files- contains all the knitted PDFs produced from analysis in the project. 

RMD File- Contains all the Rmarkdown files used for analysis for the project including geospatial analysis, plots, and time series analysis. 

## Metadata
There are four data files used for analysis:
Jackson_TenYear contains data for Fort Jackson.
KFSI_Observations contains data for Fort Sill.
KLSF_Observations contains data for Fort Benning.
KTBN_Observations contains data for Fort Leonard Wood.

Each raw data file in the Data/Raw folder contains the following data recorded in hourly increments between 2012 and 2022
Observation time: time and date observation was recorded
Year: year data point was collected 
Month: month the data point was recorded
Day: day of the month observation was recorded
Hour: hour of the day observation was recorded
TempC: temperature in Celsius. Forts Sill, Benning and Leonard Wood were recorded in Fahrenheit. 
DewPC: dew point recorded in Celsius
RELHUM: relative humidity as a percent
WBGTC: wet bulb temperature recorded in Celsius for Jackson and Fahrenheit for the other locations
FITSC: fighter index of thermal stress in Celsius 
HEATINDEXC: the heat index recorded in Celsius. 

## Scripts and code

The RMD file contains all the scripts used to carry out the analysis for the project.
MapView contains code to map the locations of the bases in the study. 
Summer_Temperature files contain code to perform time series analysis for April to September. 
Summer_Time_Series_WBGT contains scripts for time series analysis on wet bulb temperature from April to September
Temperature_Time_Series contains code for time series analysis for temperatures over the entire study period. 
Time_Series_WBGT contains code for the time series analysis for wet bulb temperatures over the entire study period. 
WBGT_HarzardousDaysAnalysis contains code for the amount of days exceeding a hazardous threshold.

## Quality assurance/quality control
All code in the final Patton_GuimondENV872_Final_Project file was examined and run by both Austin Guimond and Erik Patton. Each analyst examined the code and results of each analysis to ensure data was run properly. Any issues with code were brought up with the other analyst and resolved as needed. Code was run outside of the final report to ensure code was run properly and resulted in all the necessary data for the study. 
