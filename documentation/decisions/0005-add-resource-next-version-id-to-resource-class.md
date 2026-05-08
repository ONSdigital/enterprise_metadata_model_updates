# 5. Add Resource Next Version ID to Resource class

Date: 06/05/2026 17:13

## Status

ACCEPTED

## Context

While making an instance model to demonstrate versioning I noticed the model included a "Previous Version" identifier for Resources but not a "Next Version". dcat:nextVersion isn't a regular property in DCAT but it's an allowable inverse property and since we are already using "replaces" along with "isReplacedBy", I wanted to add it for consistency.

## Decision

To add "Resource Next Version Identifier" to Resouce.

## Consequences

Slightly more data entry/maintenance overhead, however when a next version is known (ie when it is entered) it should make it easier for systems or analysts to build a version chain.