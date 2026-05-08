# 4. Add modified DDI-CDI classes Data Structure and Variable to model

Date: 05/05/2026 17:33

## Status

PROPOSED

## Context

DORA requires us to record tables and variables within datasets at the logical level. DDI-CDI provides a standard way of doing this, however this would take a lot of research to understand and would involve creating a complex hierarchy of classes, very few of which will contain attributes for the time being. I suggest using a simplified version of this which will be overhauled in future iterations, once we have time and the need is identified (for instance it will be important for surveys later on). 

I've created the classes Data Structure and Variable in the ONS Metadata Model containing what DORA is interested in for the time being. This abstracts away DataStructureComponent, PrimaryKey, ForeignKey and a few other things. The risk of including them is that I don't understand them thoroughly anyway so they will probably need to be reworked in the future, and in the meantime the model will annoy everyone and be difficult to explain. Once these classes are fleshed out DORA can use them immediately as is with the proviso that one day it'll change.

Stakeholders for this: Samantha Iacob(proposer), Hollie Young and Lorraine Crichton (Data Architects), Rhydian Page (Data Engineer), optionally Kirti Tandel and Charles Baird (Lead and Chief Data Architect respectively).

## Decision

6/5/26 - Discussion with Hollie, Lorraine and Wilfred led to decision to remove Data Structure - the versioning and metadata requirements of tables means that they can be treated like datasets in their own right. This also maintains compliance with DDI-CDI which considers tables to be datasets, so expanding it out later will be easier. Variables will be recorded separately for now... Still need to discuss this with Rhyd.

## Consequences

6/5/26 - Variable class added to model provisionally. Data Structure not included.