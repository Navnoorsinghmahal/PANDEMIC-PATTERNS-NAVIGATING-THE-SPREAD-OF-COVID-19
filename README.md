# PANDEMIC PATTERNS: NAVIGATING THE SPREAD OF COVID-19

This repository contains the source code and documentation for the COVID-19 visualization project. The project aims to analyze and visualize the impact of the COVID-19 pandemic across different geographic regions using various data structures and algorithms.

## Table of Contents

- [Introduction](#introduction)
- [Datasets](#datasets)
- [Computational Overview](#computational-overview)
- [Instructions for Running](#instructions-for-running)
- [Discussion](#discussion)
- [References](#references)

## Introduction

For our project, we aim to analyze the effect of the COVID-19 pandemic across geographic regions. The pandemic has significantly impacted most communities worldwide, and through our project, we aim to highlight this spread of the virus across these communities. COVID-19 was a highly contagious respiratory illness that originated because of the novel coronavirus.

This pandemic caused a widespread impact on health and the economy. We believe there is a need for effective visualization of how viruses spread across communities. By looking at the coronavirus spread globally, we can understand how global economies are affected and gain more insights into the patterns and trends of the pandemic. This information will be helpful for health officials, policymakers, and the general public to make better decisions regarding disease prevention and measures.

**Project Goal:** How can we visualize the spread of COVID-19 across geographic regions of different sizes? Our goal is to create an interactive visualization tool that allows users to explore COVID-19 case data with the number of deaths and vaccination records, adjusted for population, at the continent and country levels. By combining population data and COVID-19 case data, we aim to create a detailed and informative visualization that can help users understand the impact of the pandemic and the vaccination drive on different regions.

## Datasets

We utilized the following dataset for our analysis:

- Source: [COVID-19 Data](https://github.com/owid/covid-19-data/tree/master/public/data)

We constructed a comprehensive database of COVID-19 statistics, including total cases, deaths, and vaccinations, by country and region by processing the dataset and extracting key values.

## Computational Overview

In our project, we implemented the tree data structure on our dataset, which helps us represent the hierarchical structure between the world, its regions, and their respective countries and effectively visualize the transmission of COVID-19.

- **Data Preprocessing:** Reading and wrangling the raw data file and extracting relevant information such as dates, cases, deaths, and vaccinations.
- **Tree Construction:** Building tree structures and implementing all the non-trivial recursive algorithms from scratch to represent the relationship between countries, continents, and regions over the years.
- **Data Analysis:** Computing statistics and trends to visualize them in the form of bar plots and map plots.
- **Visualization:** Developing interactive visualizations using Python libraries such as [GeoPandas](https://geopandas.org/en/stable/) and [Matplotlib](https://matplotlib.org/) to illustrate the spread of COVID-19 and associated factors.

## Instructions for Running

To run our program, follow these steps:

1. **Download all the required files** and unzip them to obtain program files and folders.
2. **Install the required Python libraries** listed in the `requirements.txt` file.
    ```sh
    pip install -r requirements.txt
    ```
3. **Execute the `main.py` file.**
    ```sh
    python main.py
    ```

Upon running the program, you will see a window pop up showing the interactive visualizations of the spread of COVID-19 statistics for the world. Additionally, there will be a play/pause button, reset button, and two sets of filters that will let you choose the region you want to visualize. Upon choosing one of the regions from the filter, you will also be able to see its respective bar plot showcasing the statistics for the countries present in that region.


## Discussion

Our computational exploration yielded valuable insights into the dynamics of COVID-19 spread and its determinants. Key findings include:

- The trend of COVID-19 cases from the epicenter to the rest of the world during the prominent 4 years of the pandemic.
- The important role that vaccines play in mitigating the effect of the pandemic by observing the trends in vaccine-intensive countries.
- The trend of the number of deaths showing compared to the number of cases, indicating the mortality rate in different regions.

Despite these contributions, our analysis has certain limitations, such as we mentioned in the project proposal that we will analyze the COVID data at state level and district level but because of the non-availability of reliable data, we were not able to do so.

## References

- GeoPandas Documentation. Retrieved from [https://geopandas.org/en/stable/](https://geopandas.org/en/stable/)
- Matplotlib Documentation. Retrieved from [https://matplotlib.org/](https://matplotlib.org/)
- Our World in Data. "COVID-19 Data." GitHub, GitHub, Inc., accessed 2 March 2024 [https://github.com/owid/covid-19-data/tree/master/public/data](https://github.com/owid/covid-19-data/tree/master/public/data)
