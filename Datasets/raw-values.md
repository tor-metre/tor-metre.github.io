---
layout: default
title: Understanding Raw Values
parent: Datasets
nav_order: 5
---

## Processed (sqlite)

Columns are ordered alphabetically. Any visual metrics, e.g. visualComplete or SpeedIndex are rounded to the nearest 100ms. 

| Column Name        | Description          | 
|:-------------|:------------------|
| SpeedIndex | The result of integrating Visual Completion over time, described in more detail here.|
| TTFB | Time to first byte (ms) | 
| URL  | The URL that was measured
| bytesIn | The number of bytes received | 
| bytesOut | The number of bytes transmitted |
| date | The timestamp of the request (Linux Epoch Time) |
| domElements | How many DOM elements were present at the end of the request. | 
| firstPaint | The time (ms) until the user saw item of content appear - i.e. was no longer looking at a blank page. | 
| label | This specifies the scenario script that the measurement belongs to. Typically it identifies any parameters applied to the session. | 
| location | This specifies the GCP instance that ran the test and the browser that was used. | 
| maybeCaptcha | Whether the page load was blocked by a CAPTCHA, according to WPT's heuristics. | 
| pages | JSON encoded URLs which link to further details regarding this request. | 
| requestsFull | How many individual HTTP requests were made in order to load this page | 
| responses_200 | How many 200 (Good) responses were received. | 
| responses_404 | How many 404 (Forbidden) responses were received. | 
| responses_other | How many responses resulted in other error codes or redirects. 
| run | This identifies which test series the measurement belongs to. Any given measurement is uniquely identified by the label, run and step |
| step | In the current session, which number measurement this was. Use the label column to identify the session. | 
| test_run_time_ms | The total time required to run the test in ms. This includes the entire session |
| visualComplete | The time until the page finished loading was no longer visually changing in ms. | 
| visualCompleteXX | XX indicates the % complete and is one of {85, 90, 95, 99}. |

## Raw (JSON)

