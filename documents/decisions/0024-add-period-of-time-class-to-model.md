# 24. Add Period of Time class to model

Date: 07/08/2026 15:58

## Status

ACCEPTED

## Context

Wilfred I identified the need for a Period of Time class in the model to allow for start dates and end dates to be grouped into a coherent collection of attributes which could be used to calculate durations. Additionally this would allow for multiple time periods to be assigned to a dataset or dataset series - in Population Statistics it's meaningful to track the duration of availability of a dataset to ONS as well as the duration of the coverage of the data. A similar approach has been taken to Frequency for the same reasons.

## Decision
Add the Period of Time class from DCAT. Make Temporal Coverage Start and End Dates and Temporal Coverage Duration generic and move them to the new class.

## Consequences
No immediate issues.