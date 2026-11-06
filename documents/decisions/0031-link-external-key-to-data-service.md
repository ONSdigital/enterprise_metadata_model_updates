---
date: '2026-11-06'
id: 5f3c6c62-10ef-43a3-bcd4-125bc9d70124
ordinal: 31
status: accepted
superseded_by: null
supersedes: []
tags: []
title: Link External Key to Data Service
---

# 31. Link External Key to Data Service

Date: 2026-11-06

## Status

ACCEPTED

## Context

James M reviewed the model and when talking to Sam I asked about the External Key class. This is intended to link datasets in the catalogue to systems maintained outside the catalogue, for instance APIs and registries, and the "Type" property was meant to be a controlled list of these systems. However these systems are exactly what should be recorded in Data Service, making such a controlled list unnecessary. 
 
## Decision

External Key link to Resource removed. Linked to Dataset and Data Service instead (as an associative class). External Key Identifier removed from the primary key and changed to External Key String. External Key Type deleted from the model.

## Consequences

One less "Type" list to control. The class is superficially similar to Dataset-Data Service Access (another associative class between Dataset and Data Service) but has a different purpose. Access shows that a distribution of a dataset is accessible through a particular data service, while External Key is mostly about linking to additional metadata or what-have-you associated with a catalogued dataset (but which is maintained separately) and doesn't necessarily imply that a distribution is available through that service.

This does mean that data services that don't hold distributions (such as registries) HAVE to be recorded as Data Services for the catalogue to hold an external key for them.

This is designed for internal systems only, the External bit just means "external to the catalogue".