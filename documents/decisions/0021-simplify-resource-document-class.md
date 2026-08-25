# 21. Simplify Resource Document class

Date: 04/08/2026 14:37

## Status

ACCEPTED

## Context

Developing the governance and provenance layers revealed that the Resource Documentation would have to be linked up to the attribution system (ie someone had a role in a document) to remain consistent with the rest of the model. This led Sam I to look it over and realise that the resource document class just requested too much information about what should essentially be a link to a word document or something somewhere and that this information wasn't requested or likely to meet any needs that had been identified so far. Essentially we would end up with a lot of NULLs and while it would retain a limited capability to do version control and assign ownership to documents, this could be done better and easier in whatever storage solution is actually holding them.

## Decision

Strip most of the attributes out of the Resource Document class but add an optional "Valid From" and "Valid To" date. Sam I took this decision alone.

## Consequences

To simplify the model. If in the future there's an identified need for a more robust documentation system (ie some documents should be catalogued) this would be better done by creating a documentation class or classes as a subtype of Resource.