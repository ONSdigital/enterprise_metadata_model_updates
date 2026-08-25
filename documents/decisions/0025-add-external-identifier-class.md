# 25. Add external identifier class

Date: 11/08/2026 13:43

## Status

ACCEPTED

## Context

Feedback MRD-047 in the DORA feedback register identified the a requirement to hold IDs to external catalogues/registries/libraries etc such as IDAR, Business Catalogue and so on. Sam I had resisted this previously as the catalogue was meant to replace these other registries, but as the catalogue implementation has been descoped this seems less likely than it did intitally. 

IDAR number was a candidate for inclusion in future updates anyway but as multiple of these may be required before a catalogue it would be useful to model these identifiers so that any number of them can be associated with a resource, rather than creating new properties at the logical level (which would be an anti-pattern because it would limit the number of the identifiers that could be associated, and there always seem to be more of them or at least there could always be more if people keep making catalogues of things).

Recommend creating a class called External Key (based on adms:Identifier), containing the minimum properties:

Resource ID 
Identifier (ie the IDAR number)
Identifier Type (IDAR, Business Catalogue, Admin Data Library, whatever else).

Cardinality : Each Resource can have zero, one or many External Keys.

Strictly speaking Identifier Type could link to a Catalogue class now that we're not just building a single catalogue but modeling a bunch of catalogues that interact with other catalogues (and stepping back into Mandy's catalogue of catalogues territory!). In the interest of simplicity Sam doesn't want to think about it but it could be a consideration for the future.
 
## Decision

It's been added to the model.

## Consequences
Allows us to take advantage of existing catalogues and other metadata systems while we wait for a catalogue (and buys us time to think about how to deal with requirements without simply adding attributes somewhere in the model)
