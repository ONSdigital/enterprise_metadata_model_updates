# 3. Add CatalogRecord class to model

Date: 01/05/2026 09:56

## Status

ACCEPTED

## Context

DORA requires the ability to distinguish between the date a dataset is made available (ie its publication date or date of acquisition by ONS) and the date and time a record is created in the catalogue. DCAT provides for this with CatalogRecord which is an optional class that exists for this purpose. 

## Decision

Rhyd, Hollie, Lorraine and I decided to include the CatalogRecord class in the ONS metadata model.


## Consequences

The class will be added to the model and allow the catalogue to hold records about the registration of resources such as datasets, data services and dataset series. It will not appear in the domain profiles of areas that don't require it.