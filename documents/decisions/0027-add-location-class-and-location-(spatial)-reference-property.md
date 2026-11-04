---
date: '2026-10-28'
id: 09f853e3-b459-48a6-996d-d9e02ff6350d
ordinal: 27
status: proposed
superseded_by: null
supersedes: []
tags: [geography, ]
title: Add Location class and Location (spatial) Reference property
---

# 27. Add Location class and Location (spatial) Reference property

Date: 2026-10-27

## Status

PROPOSED

## Context

Meeting between Louise B, Wilfred I, Lorraine C and Sam I. Louise had identified that the way geography was handled in the model (descriptive highest and lowest geographies was simplistic and wouldn't meet the needs of researchers. There was also some ambiguity around "spatial resolution/granularity" as it was mixing up a descriptive resolution attribute with the reference (the way each unit of those resolutions are referenced in the data - for instance, a MSOA could be referenced by latitude or longitude, or more controversially a postcode etc).

During the conversation it was also revealed that a dataset or dataset series may feature multiple layers of geography, and each may have its own distinct reference.

## Decision

The geography information in dataset to be moved to its own class and a distinct Reference property added there. Each dataset and dataset series must be associated with at least one geography. This class has been named Location as is normal for DCAT etc, but it holds slightly different properties. This can be expanded in future to contain geographic data (boundary data, centroid etc) if desired.

Coverage (defined as the spatial/geographical area or jurisdiction covered by the dataset) is mandatory, Granularity and Reference may be null. This is to allow a dataset series to hold very basic information about the country or territory covered by the dataset.

## Consequences

Code lists will need to be established for Coverage, Granularity and Reference. Coverage in particular is likely to be challenging as ONS doesn't have a taxonomy of geographies at present. There is some controversy about whether "Postcode" can or should be used to denote Granularity or Reference - more expert advice will be needed on this.

In the meantime we can probably derive code lists from IDS - the granularity and reference ones will need to be split out. 