# 14. Remove 'hard coded' actors from Resource class

Date: 19/06/2026 12:04

## Status

ACCEPTED

## Context

There are some "hard coded" actor types in the Resource class which was a concept inherited from DCAT-UK for the minimal possible amount of metadata. These were intially designed to simply be an email address for the resource creator, contributor and contact point which would be the data steward. It became clear though that more information is required on those roles. The addition of Contributor as a hard-coded actor type for digital publishing also points to the likelihood that more of these will be required in future if this isn't nipped in the bud. Also in practice it means there's likely to be duplication as ContactPoint is filled in and someone attached to a resource as a Data Steward via the agent/role/attribution system, which could lead to confusion down the road.

## Decision

Remove all hard-coded roles (Creator, ContactPoint and Contributor), rely on the agent/role/attribution system for all roles in relation to a catalogued resource. If this needs to be selectively violated at the physical level it can be (for instance having a Creator/Contributor field in Dataset which points directly to the Actor table) it can be done in a controlled manner.

This decision was taken by Sam I on her own. It supercedes decision 0010 which defined the creator, contributor and contactPoint properties in terms of what agents they represent.

## Consequences

This should reduce ambiguity in desk instructions and allow for multiple of the same kind of role to be involved in a resource (ie, multiple contributors) at the cost of slightly more complexity. However as information such as name as well as email are usually required it was probably unavoidable to use the Agent class, and in that case an associative entity would have been needed to prevent a many-to-many relationship.