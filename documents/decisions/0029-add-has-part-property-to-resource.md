---
date: '2026-11-04'
id: 3b899e3d-62a9-4731-8d5a-7565b018bc37
ordinal: 29
status: proposed
superseded_by: null
supersedes: []
tags: []
title: Add Has Part property to Resource
---

# 29. Add Has Part property to Resource

Date: 2026-11-04

## Status

ACCEPTED

## Context

Related Resource was a class that was supposed to catch all relationships between catalogued resources using a "type" attribute. However it was downgraded as no use was identified for it outside of Dissemination/Digital Publishing, who only needed to know that two or more datasets were related without any additional information.

However in IDAR world datasets can be part of other datasets - for instance, lots of datasets make up the Demographic Index. DCAT has a standard way to capture this relationship - "has part" (and its inverse, "is part of"). This was always an intended use of Related Resource.

## Decision

Sam I decided to add this back into the model as a property in Resource.

## Consequences

This should allow datasets to be part of other datasets as and when this is needed.
