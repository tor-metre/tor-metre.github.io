---
layout: default
title: Guard Variance Run
parent: Datasets
nav_order: 3
---

## Motivation / Summary

This dataset was gathered to look for possible differences in performance between Tor Browser Client Instances. Tor Browser Instances select a list of guards and a preferred guard on their first start up. As exit nodes are known to vary widely in their performance, the same may be true of guard nodes. 

## Dataset Description

| Parameter | Description          | 
|:-------------|:------------------|
| Locations | US Central |
| Browsers |  Firefox, Tor Browser |
| Time Range | 13th August 2019 18:05 GMT to 20th August 23:27 GMT |  
| Page Source | 72 domains selected from the Alex Top 10,000. 25 from the top 100, 23 from the bottom 1000, 25 in between |
| Add-ons | None |
| Scenario | Short sessions consisting of navigating to a home page directly, then clicking a single on the loaded page which stayed on the primary domain.   |
| Runs | 200 Tor Browser Instances, 2 Firefox Instances |
| Total Present Samples | ~600 000 |

## Known Problems (if any)

Approximately half the samples are not valid due to an error in their version of the Tor Browser. These invalid samples contain "tor-with-timer" in their location string. This bug causes an incorrect timing measurement when the "tor-with-timer" Browser instance is used with Ublock origin. 

Some samples contain missing values indicated by the string "MISSING"

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
