# 20. Change Revision entity to Derivation in provenance layer

Date: 31/07/2026 10:35

## Status

ACCEPTED

## Context

Discussion between Sam I and Lizzie F (data architects). The model has a class called "Revision" which relates resources (mostly datasets) to the resources they are revised from. In the Provenance ontology and data model, Revision is a specialisation of Derivation which adds the requirement that "substantial" content from the original source is used. Sam I selected this as our revised datasets should meet this condition and because none of the other specialisations of Derivation (primary source and quote) apply to the catalogue.

However Lizzie pointed out that the business already uses the term "Derivation". Sam I responded in the trademark way that doesn't make her lots of friends that "she doesn't care what the business calls things", but the point was taken. Sam and Lizzie also came to the conclusion that there might be a need for other types of derivation in the future so it might be simplest to take the widest possible option for now. 

## Decision

Revision class changed to Derivation in the model and definition updated.

## Consequences

As this isn't in production yet it's not going to cause any issues.