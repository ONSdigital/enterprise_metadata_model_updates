# 23. Add Dataset Type property

Date: 06/08/2026 14:56

## Status

ACCEPTED

## Context

As DORA (probably) will roll the subtypes of Resource up, the Resource Type property will be needed to differentiate between which subtype of Resource is being catalogued. An additional type is required for Dataset to allow DORA to have different types of dataset.

## Decision

To add Dataset Type as a new property (within the Dataset class, meaning "type of dataset") and tighten the Resource Type definition to make it clear that this type relates only to sub-types of Resource.

## Consequences

Datasets and Dataset Series can pick an additional type. Unsure if there will be a single enumerated list of types that will suffice for the whole organisation or if it eventually needs to be linked to a taxonomy via a concept scheme in future but leaving that alone for now.