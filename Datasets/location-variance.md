---
layout: default
title: Location Variance Run
parent: Datasets
nav_order: 3
---

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

[Compressed Sqlite File](TODO)
