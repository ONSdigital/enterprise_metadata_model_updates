# 18. Simplify provenance layer

Date: 27/07/2026 11:39

## Status

ACCEPTED

## Context

Initial investigation of the PROV-DM (provanance vocabulary data model) suggested several classes that could potentially be useful. Sam I modeled the ones that she felt would be possible to implement within a relatively simple lineage system and showed the working group (Hollie Y, Charles B, Wilfred I, Lorraine C). In the discussion it became clear that initially data entry for lineage would probably be manual which meant that optionally classes such as Generation and Usage which provided extra context around the creation and modification of datasets would be difficult to manage.

## Decision

To remove the optional classes from the model and to make it as simple as possible.

## Consequences

These classes (along with other ones already not included because of complexity such as Communication and Plan) will probably need to be investigated again in future when we have an automated system in place that can generate and read lineage information.