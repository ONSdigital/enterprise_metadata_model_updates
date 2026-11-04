---
date: '2026-11-04'
id: 54e21d4c-127c-4aa1-b22b-4c06f8c2fe84
ordinal: 30
status: proposed
superseded_by: null
supersedes: [0014]
tags: []
title: Restore Creator, Publisher and Contact Point properties to Resource
---

# 30. Restore Creator, Publisher and Contact Point properties to Resource

Date: 2026-11-04

## Status

ACCEPTED

## Context

DORA (Neal J and Tim O specifically) needed a quick way to refer to the creator, publisher and contact for a dataset without reference to a codelist of roles. Since these roles are present in nearly all datasets and are expected by most standards, Sam I owned up to getting a bit too cute with her logical modeling and inadvertently causing confusion. The agent/role/attribution system is suitable for other functions carried out for catalogued resources and codelists etc but should not be employed for the most basic cases where a direct attribution (from resource to agent) works fine.

## Decision

Restored the Creator, Publisher and Contact Point properties and linked them directly to Agent (and its subtypes)

## Consequences

This should make the engineers' life easier and stop people asking "where's the dataset creator attribute?", a question which is exhausting to answer with reference to the agent/role/attribution system.