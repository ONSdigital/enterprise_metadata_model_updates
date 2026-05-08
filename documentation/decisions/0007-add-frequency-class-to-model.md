# 7. Add Frequency class to model

Date: 08/05/2026 15:19

## Status

ACCEPTED

## Context

There is a need to record multiple different types of frequency (recurrence) in relation to datasets, and these differ across the business. Some examples include "publication frequency" and "delivery frequency". DCAT by default has frequency as a property of the Dataset class but it would be a bad idea to create numerous typed frequency attributes as most of these would be null in most datasets and it's likely we'd need to add more over time.

DCAT-AP offers a supporting class to deal with this situation called "Frequency". The types of aloowable frequencies and the actual frequency description (ie "annual", "weekly" etc can be controlled by ontology.

## Decision

To create the Frequency class as a child of Dataset. Contributors : Lorraine Crichton, Wilfred Inuaghata, Sam Iacob

## Consequences

This allows for multiple frequencies of different types for datasets but requires the lists of frequency types to become a controlled vocabulary. It deviates from DCAT's UK implementation which only allows for updateFrequency which relates to the frequency of publication. This might make interoperability across government catalogues slightly iffier but I don't think it's a huge deal really. If necessary could reintroduce "updateFrequency" to the dataset to get around this issue.
