# 11. Add temporal dimensions to Attribution class

Date: 19/05/2026 13:58

## Status

ACCEPTED

## Context

The Attribution class allows for any number of roles and agents to be related to a catalogued resource. It isn't currently possible to track who held what roles in the past. Adding attribution start and end dates will allow us to keep track of who was involved with a dataset or data service and when that was. 

## Decision

As this was in Mandy's model and is a trivial addition it was added to what will be version 1.4 of the model, from Erwin version 22 onwards.

## Consequences

This will improve the capabilities of the catalogue without creating much overhead - attribution start and end dates/timestamps can be entered manually or programatically. 