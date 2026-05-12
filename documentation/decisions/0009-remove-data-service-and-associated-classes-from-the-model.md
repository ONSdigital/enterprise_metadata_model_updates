# 9. Remove Data Service and associated classes from the model

Date: 12/05/2026 14:14

## Status

PROPOSED

## Context

During the metadata model/ontology meeting on 12/5 Sam I expressed concerns about the data service class in the model and how it related to datasets and distributions. The way their relationship is modelled as of v 1.2 is possibly a misunderstanding of the DCAT standard. Also as data services are not currently a required part of the model for DORA or DS-DP it isn't likely to feature in their APIs and so will not form part of their domain profiles.

## Decision

It would be a good idea to remove Data Service, its relationships and associative classes from the model for the time being. While these are likely to be important in the future it would be better to simplify the model until it's necessary to add classes for a domain. It would also save designing time on researching the correct way to implement the data service class when it isn't needed (presumably this time will be available later, when it is)

This will be discussed with James A, a technical architect, to see whether the class is vital or can be dropped for now. 

## Consequences