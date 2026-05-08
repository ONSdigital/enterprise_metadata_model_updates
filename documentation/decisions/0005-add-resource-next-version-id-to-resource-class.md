# 5. Add Resource Next Version ID to Resource class

Date: 06/05/2026 17:13

## Status

PROPOSED

## Context

While making an instance model to demonstrate versioning I noticed the model included a "Previous Version" identifier for Resources but not a "Next Version". dcat:nextVersion isn't a regular property in DCAT but it's an allowable inverse property and since we are already using "replaces" along with "isReplacedBy", I wanted to add it for consistency and to make it easier to build version chains.

## Decision

To add "Resource Next Version Identifier" to Resource? I've added it for now

8/5/26 - I've talked to Keith (senior DA) and he said that it's an abnormal choice for this kind of model, as the catalogue can build a version chain by starting at the current version and working backwards. The Resource Next Version ID might be overkill as while it's allowed by DCAT it's not the default behaviour.

## Consequences

