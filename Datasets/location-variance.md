---
layout: default
title: Location Variance Run
parent: Datasets
nav_order: 3
---

## Motivation / Summary

This dataset was gathered in order to evaluate how Tor's performance varies with geographic location. It measures a range of websites, with/without Ublock, using both Firefox and Tor Browser. The geographic locations are chosen from Google Compute Engine's list of data centres and consequently represent a "best case" for a Tor user in that region. 

## Dataset Description

| Parameter | Description          | 
|:-------------|:------------------|
| Locations | Tokyo, Singapore, Mumbai, Sydney, Finland, London, Frankfurt, Sao Paulo|
| Browsers | Firefox, Tor Browser  |
| Time Range | Wednesday, 28 August 2019, 18:26->22:54 GMT|  
| Page Source | 72 domains selected from the Alex Top 10,000. 25 from the top 100, 23 from the bottom 1000, 25 in between |
| Add-ons | With/Without Ublock Enabled.|
| Scenario |  Short sessions consisting of navigating to a home page directly, then clicking a single on the loaded page which stayed on the primary domain. |
| Runs | Each measurement was gathered twice |
| Total Present Samples | ~13,000|

## Known Problems (if any)

Some rows contain missing values, which are denoted "MISSING". These rows should be ignored as the reason for the missing data is not known. Consequently this dataset cannot be used to infer any statistics about failed requests. However, it can be used to infer statistics about successful requests. 

Even though there were two runs of this experiment, the runs column is incorrectly set to zero for each measurement.

## Filtering on Parameters 

| Parameter | Source Column          | 
|:-------------|:------------------|
| Locations | Location |
| Browsers | Location |
| Time Range | Date|  
| Page Source | URL |
| Add-ons | Label|
| Scenario |  Label |



## Download

[Compressed Sqlite File](https://www.jottacloud.com/s/1539e9992a4d98d4d3396cd6e5894082d15) - 1.6 MB

