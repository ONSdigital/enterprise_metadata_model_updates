# 6. Add Literal class to handle alerts

Date: 07/05/2026 17:49

## Status

ACCEPTED

## Context

DS-DP requires an alerts function but there is no standard DCAT or DCAT-UK class to handle annotations that I could find. I looked into DCAT-AP, the European implementation of DCAT, and found a Literal class which would seem to allow usage as an annotation. 
I've included this in the model as a child of the Resource class. This would allow non-alert annotations to datasets that other teams might find useful in future.
Stakeholders for this decision are DS-DP and the EMM architects as a group. - SI

## Decision

TBC after discussion with EMM architects

UPDATE 8/5/26 - I talked about this briefly with Charles. Unsure about DCAT-AP classes but for now I can't see an easy way around this other than to just not model alerts. This might be why Mandy didn't include them? 

Also thought about whether this should sit at the dataset level rather than resource, which would let datasets and dataset series use them... not sure, would data services have a use for annotation? 

The issue here is about how or whether to incorporate all requirements into the model... each business area will have some niche demand for the catalogue to handle. I don't particularly see the harm as long as the domain profiles are put together properly.

Following discussion on 12/5 it was decided to keep the Literal class.  The class has been renamed to Annotation to capture what it is supposed to be doing a bit better. 

## Consequences

DS-DP are able to have alerts and usage notes as they wanted, so it will mean fewer changes for them. The class can be extended with different Annotation Types in future to meet other requirements in future.