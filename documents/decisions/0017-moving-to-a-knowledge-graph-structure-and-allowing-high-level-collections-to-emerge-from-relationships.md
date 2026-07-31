# 17. Moving to a knowledge graph structure and allowing high-level collections to emerge from relationships

Date: 10/07/2026 17:00

## Status

ACCEPTED

## Context

Stakeholders: Rhyd P, Charles B, Hollie Y, Wilfred I, Lorraine C, Lizzie F, Sam I 

There was some debate about how collections should be managed in the metadata model - as dataset series, dataset, catalogues etc, and how these should be defined. Some issues included differences between how business areas conceive of "collections" - whether parent-child relations, buckets of links to all associated datasets, or not used at all.
 
Rhyd P showed a prototype he made using BigQuery Graphs which was configured as a knowledge graph based on the metadata model. He demonstrated some impressive capabilities for determining association between entities using the model logic rather than requiring intentional grouping. This would allow a lot more flexibility than a relational structure (essentially allowing for an evolving data model and allowing business areas to structure how their datasets are grouped without requiring business-wide changes). 

## Decision

24 hours were given for participants to raise issues and none were raised. DORA will implement the model as a knowledge graph and allow "collection" to emerge from relationships within the model.

## Consequences

This puts some priority on developing a provenance model otherwise the relationships won't exist for anything to emerge from.