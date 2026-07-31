# 5. Add Resource Next Version ID to Resource class

Date: 06/05/2026 17:13

## Status

DEPRECATED

## Context

While making an instance model to demonstrate versioning I noticed the model included a "Previous Version" identifier for Resources but not a "Next Version". dcat:nextVersion isn't a regular property in DCAT but it's an allowable inverse property and since we are already using "replaces" along with "isReplacedBy", I wanted to add it for consistency and to make it easier to build version chains.

## Decision

To add "Resource Next Version Identifier" to Resource? I've added it for now

8/5/26 - I've talked to Keith (senior DA) and he said that it's an abnormal choice for this kind of model, as the catalogue can build a version chain by starting at the current version and working backwards. The Resource Next Version ID might be overkill as while it's allowed by DCAT it's not the default behaviour.

12/05 Discussion between Charles B, Kirti T, Lorraine C and Sam I. : outcome was that there are pros and cons to this. Planning to talk to James Anderson to discuss the tradeoff between ease of integration and increased risk of data entry/update errors.

15/5 We did not actually discuss this at the meeting. As a result, following senior data architect advice (Keith), and creating an instance model that showed that these properties are not strictly necessary the inverse properties were removed from the model. 


## Consequences

The model is simpler to understand and should still be functional. The relationship lines are now labelled reciprocally instead. If the inverse properties are required for any classes this decision can be revisited and the inverse properties restored.