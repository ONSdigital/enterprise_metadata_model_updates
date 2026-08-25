# 26. Add Category-Taxonomy class in Governance layer

Date: 14/08/2026 16:54

## Status

ACCEPTED

## Context

The Governance layer of the model is used for assigning domains, subdomains, themes and other categorisations to catalogued resources. It's a simplification of SKOS that allows for simple hierarchies of concepts, where narrower concepts can only be part of a single broader concept (for example in an animal taxonomy, a Cat could be a narrower concept of Mammal). In discussion between Rob G (digital publishing) and Sam I it was revealed that there may be a need for a concept to belong have multiple broader concepts - for instance, datasets about COVID could be a sub-theme of Health, Population, Economics etc.

It should be noted that in the model the class managing this is called Category rather than "Concept" to make it clear what the purpose of the class is, but it is aligned to SKOS:Concept

## Decision

To replace the simple "Parent Category Identifier" in the Category class with an associative entity called "Category-Taxonomy" which allows for a many-to-many relationship between categories. 

## Consequences

The model is slightly more complicated but this should meet the requirement to have cross-cutting sub-domains, sub-themes and sub-categories linked to multiple broader categories. 