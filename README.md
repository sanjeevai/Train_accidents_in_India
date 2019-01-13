# Train Accidents in India

## [Blog version](https://medium.com/@sanjeevai/train-accidents-in-india-c1b0f180b2d2)

## Table of Contents
- [Project Overview](#overview)
- [Data](#data)
- [Files](#files)
- [Results](#res)
- [R libraries](#rlib)
- [Python libraries](#pythonlib)
- [Python vs R](#pythonr)
- [Limitations](#lim)
- [Acknowledgments](#ack)

***

<a id='overview'></a>
## Project Overview

Train is the most common mode of travel for long distance journey in India. This year India has seen major accidents in railways due to several factors including natural causes and human error. We have tried to study the causes of train accidents for year 2002-2017, and other factors which trigger train accidents in different parts of the country. This report includes major accidents till 2017 which impacted the customer experience or say made it unsafe to travel in train.

<a id='data'></a>
## Data

Data was collected from various news websites, online news archives, [Wikipedia articles](https://en.wikipedia.org/wiki/List_of_Indian_rail_accidents), etc. Data was available on the internet from year 1890-2017 but analysis is carried out for 2002- 2017 because news reports on many old incidents needed citations and some of them were reported in less detail on news websites. To cover major features affecting the accident rate in India and to closely compare them, 2002-2017 year range provided enough observations (114) to make some statistical conclusion.

<a id='files'></a>
## Files

* abbreviations.md

Contains abbreviations used in this project.

* DoMS_2.5.2.csv

Input data with 9 features and 114 observations.

* project.ipynb

Data analysis in Python. This was required for project submission in **Udacity's [Data Scientist Nanodegree](https://in.udacity.com/course/data-scientist-nanodegree--nd025) program**. It contains the same results as in *report.rmd* file but in less depth.

* report.rmd

Here I performed the main part of the project in R. That includes:

* Data Pre-Processing
* Feature engineering
* Feature selection
* Exploratory Data Analysis
* Hypothesis Testing

* report.pdf

It is the PDF export of **report.rmd**

<a id='res'></a>
## Results

From the data of 16 years, it is clear that some causes can be prevented and some can't. Natural causes are very rare in causing accidents. Every year train accidents take place and exact cause of accident is not known in many cases. If the investigation of accidents are carried out in more depth then improvements can be made effectively. Accidents happening inside train, like fire, are less nowadays. Human negligence is major cause and will remain the cause in future if no special attention is given by train drivers, roadways riders, people crossing tracks, vehicles crossing tracks, etc. 

<a id='rlib'></a>
## R libraries

* ggplot2
* lubridate
* gtools
* gsubfn
* plyr
* tidyr
* dplyr
* gridExtra
* qcc

<a id='pythonlib'></a>
## Python libraries

* pandas
* numpy
* datetime
* matplotlib
* scipy
* seaborn

This project uses Python 3.

<a id='pythonr'></a>
## Python vs R

You might be thinking why I did this project in both **Python and R**. The reason is that I often choose R over Python when there is no machine learning involved in the project. For statistical analysis, R seems more intuitive and compact. The goal of this project was **factor analyis**, and it did not require any machine learning algorithms at this stage.

I created Python version because it is a requirement of the the first project in **Udacity's Data Scientist Nanodegree Term 2**.

<a id='lim'></a>
## Limitations

There are some limitations of this data:

* it was not possible to account for each accident because of very brief report of some incidents on news websites

* this report does not address solution for external attacks

* condition (old or newly launched) of trains is not known

* this report addresses accident counts over years 2002-2017. It does not analyse trends in casualties because we wanted to prevent them directly by knowing the cause of accidents.

<a id='ack'></a>
## Acknowledgments

This project was not possible without the supervision of _[Prof. J. K. Nayak](https://www.iitr.ac.in/departments/DM/pages/People+Faculty+Jogendra_Kumar_Nayak.html), Department of Management Studies, IIT Roorkee._ He guided me and readily clarified all the doubts that I encountered.
