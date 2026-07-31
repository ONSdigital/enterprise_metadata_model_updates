# 15. Remove Variable class

Date: 19/06/2026 12:42

## Status

ACCEPTED

## Context

The Variable class was introduced as a temporary measure to address a need for DORA to collect some basic schema information on its datasets. As it's improperly aligned to its relevant standard (DDI-CDI) it has caused some confusion in other areas while not actually addressing any of their needs to capture schema information. DORA has since disabled its forms for capturing schema information so this no longer serves a purpose in the model.

## Decision

Sam I and Wilfred I decided to remove the Variable class.

## Consequences

This shouldn't have any immediate impacts other than to simplify the model. Introducing schema or variable level metadata is complex and should be done carefully as many business areas will require it.