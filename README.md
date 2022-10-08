# Homework 1: Professionalism & Reproducibility 

The goal of this project is to analyze the monthly articles views of a set of Wikipedia articles through the period of January 1, 2015 to October 1, 2022. We use the Wikimedia REST API to acquire the page views of various articles, which are included in the [dataset](https://github.com/reeya26/data-512-homework_1/blob/main/data/dinosaur_genera.cleaned.SEPT.2022%20-%20dinosaur_genera.cleaned.SEPT.2022.csv).

This repository contains the data files, code and results of Homework 1, for the course Data 512: Human Centered Data Science.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/reeya26/data-512-homework_1/blob/main/LICENSE) ![Language](https://img.shields.io/badge/language-python-blue.svg)

## Resources Used
- Editor used: Jupyter Notebook
- Python version: 3.9.4
- Packages used: json, time, requests, urllib, pandas, seaborn, matplotlib


## Data 

Source Files:

- [Dinosaur articles](https://docs.google.com/spreadsheets/d/1zfBNKsuWOFVFTOGK8qnTr2DmHkYK4mAACBKk1sHLt_k/edit?usp=sharing)
This dataset contains the list of Wikipedia Article names along with website links
- [Wikimedia REST API](https://wikimedia.org/api/rest_v1/#/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end) The API is used to pull-in the Page Views for each Article Title. Licensed under the [CC-BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) and [GFDL](https://www.gnu.org/copyleft/fdl.html)

Intermediary Files:

- desktop_dict: Stores the result of the API Access call, where the articles have been accessed via a Desktop
- mobapp_dict: Stores the result of the API Access call, where the articles have been accessed via a Mobile Application
- mobweb_dict: Stores the result of the API Access call, where the articles have been accessed via a Mobile Website
- total: Stores the cummulative sum of all the above dictionaries

## Project Organization

This package has the following structure.

```
data-512-homework_1/
  |- license
  |- readme.md
  |- data/
    |- dinosaur.genera.cleaned
  |- json/
    |- dino_monthly_cumulative_201501_202209.json
    |- dino_monthly_desktop_201501_202209.json
    |- dino_monthly_mobile_201501_202209.json
  |- results/
  |- Analyzing_Monthly_Article_Traffic
    
```
    
    
## Results

We obtain two results from this analysis.


#### 1. List of Dictionaries saved as Json files


- [Monthly desktop access](https://github.com/reeya26/data-512-homework_1/blob/main/json/dino_monthly_desktop_201501_202209.json) : Monthly desktop page traffic is based on one single request.
- [Monthly mobile access](https://github.com/reeya26/data-512-homework_1/blob/main/json/dino_monthly_mobile_201501_202209.json) : The API separates mobile access types into two separate requests, summing these to make one count for all mobile pageviews.
- [Monthly cumulative](https://github.com/reeya26/data-512-homework_1/blob/main/json/dino_monthly_cumulative_201501_202209.json) : Monthly cumulative data is the sum of all mobile, and all desktop traffic per article.

#### 2. Visualizations based on the analysis
 

 
 

