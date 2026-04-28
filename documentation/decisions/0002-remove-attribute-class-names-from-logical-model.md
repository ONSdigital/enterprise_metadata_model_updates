# 2. Remove attribute class names from logical model

Date: 28/04/2026 17:13

## Status

ACCEPTED

## Context

The ONS conceptual and logical modelling standard requires that attributes in logical models include the attribute class to which the attribute belongs (for instance, if a dataset theme was selected from a code list it would be called "Dataset Theme Code". However this has proven to be confusing to data architects working on the model and is difficult to explain to business stakeholders, and it interferes with generating a physical schema which is compliant with cross-government standards (and also makes it unlikely that the physical fields would be machine readable).  Sam Iacob and Hollie Young had a quick conversation about this on 28/4 to come to a solution.

## Decision

To remove the attribute class names in the attributes.

## Consequences

Attribute class names removed and will no longer be included in this model except where they add clarity. The ONS metadata model is no longer strictly compliant with the logical and conceptual modelling standard but is easier to interpret.