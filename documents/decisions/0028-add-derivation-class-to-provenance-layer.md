---
date: '2026-11-04'
id: 19bfdd36-bc60-4f07-afdf-2d5f921233f9
ordinal: 28
status: proposed
superseded_by: null
supersedes: []
tags: []
title: Add Derivation class to Provenance layer
---

# 28. Add Derivation class to Provenance layer

Date: 2026-11-04

## Status

PROPOSED

## Context

The provenance layer in the model allows for a basic tracking of how datasets are generated, used (to create other datasets) and invalidated, but derivation has been left out due to complexity. However it is a vital concept for the IDAR as it relies on parent-child relationships between assets, which are all derivations. Making this relationship explicit in the model will make transfer of IDAR relationships over to a system based on this model more or less seamless without recourse to Activity, which is unlikely to be provided for existing assets as the provenance system has not yet been used and it may be an unreasonable ask on clerical teams to supply this information.

This was discussed between Sam I and Wilfred I during a team-wide exercise and both agreed to implement this. Sam was worried about the added complexity as the model had not yet been tested using the first components (entities and activities) and Derivations belongs to component 2 of the Provenance data model (see https://www.w3.org/TR/prov-dm/#data-model-components for more information) but the value of adding it for our use case was greater than any possible downside from the added complexity.

## Decision

Derivation class added to the model on the Provenance layer. Links to the Usage, Generation and Activity classes are optional (as in the Provenance DM) - in future these may be populated but for now it's not expected.

## Consequences

Datasets may now be related to one another directly as "derivations", mirroring the parent-child relationship in IDAR, with less requirement to specify the activity that caused that derivation. In future these activities may be specified if desired.