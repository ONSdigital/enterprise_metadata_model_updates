# 10. Define contactpoint and creator roles

Date: 12/05/2026 14:24

## Status

ACCEPTED

## Context

ContactPoint and Creator are properties of the Resource class. While there is a Agent/Role system which allows for more detailed roles and full contact details for individuals and groups involved in a resource, these are (theoretically) mandatory properties which quickly indicate who is responsible for creating/publishing the dataset, and who you should email about it, respectively.

These were discussed at the metadata/ontology meeting on 12/5/26. The options were to remove them and let the agent/role system handle them, or to leave them in and define what the creator and contactpoint were.

As these are expected entries for a minimal dataset that would let a resource be (DCAT-)compliantly catalogued without recourse to the agent/role/attribution entities, it was decided that these should be kept. 

Charles B proposed that the contactpoint should be the data steward (as the owner is likely to be SCS and not easy to reach). Sam I proposed that the creator remained the "the business entity responsible for creating or compiling the original content of an information resource."

There is another role in the Resource class called "Contributor" which is required by DS-DP which is "An entity responsible for making contributions to the resource." This cannot be the same entity as the creator. This wasn't discussed in the meeting but could remain in Resource.

## Decision

To define ContactPoint as the Data Steward (when used in relation to a dataset or dataset series). 

Present: Charles B, Kirti T, Lorraine C, Sam I

## Consequences

Minor change to the definition of ContactPoint. 

It previously read : Relevant contact information for the catalogued resource. Use of vCard is recommended.

It now reads : Relevant contact information for the catalogued resource. For a dataset, this should be the Data Steward. Use of vCard is recommended.

(as an aside, we have not used vCard for these properties - they are intended to be a name or an email address. To use vCard, the role should be set up using the Agent/Role/Attribution structure which allows capturing additional details about people, teams and organisations involved in a data resource)