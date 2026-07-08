# Model Updates

This is a repository for people to access artifacts around the ONS enterprise-wide **metadata model** and any **domain profiles** created from it.
This will include reports, documentation, instance diagrams and any other thing useful for understanding the model.
It will typically be updated on (or near) Fridays whenever an update is required..


The models and reviews are (at least temporarily) [mirrored on ONS SharePoint](https://officenationalstatistics.sharepoint.com/sites/Metadata/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FMetadata%2FShared%20Documents%2F1%2E%20Enterprise%20Metadata%20Management%20%28EMM%29%2FEMM%20Workstreams%2FONS%20Metadata%20Model&viewid=22b51cd2%2D15c6%2D4d18%2Dbc10%2Dbc9e433ec574&newTargetListUrl=%2Fsites%2FMetadata%2FShared%20Documents&viewpath=%2Fsites%2FMetadata%2FShared%20Documents%2FForms%2FAllItems%2Easpx) if you need to share with anyone who doesn't have an ONS Digital account. [🔗Link](https://officenationalstatistics.sharepoint.com/sites/Metadata/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FMetadata%2FShared%20Documents%2F1%2E%20Enterprise%20Metadata%20Management%20%28EMM%29%2FEMM%20Workstreams%2FONS%20Metadata%20Model&viewid=22b51cd2%2D15c6%2D4d18%2Dbc10%2Dbc9e433ec574&newTargetListUrl=%2Fsites%2FMetadata%2FShared%20Documents&viewpath=%2Fsites%2FMetadata%2FShared%20Documents%2FForms%2FAllItems%2Easpx)

## Introduction

The ONS metadata model describes an enterprise data catalogue which is based on international standards and identified requirements from business areas that will be interacting with it. To deliver this as quickly as possible it is being built in a top-down and bottom-up way at the same time. The model as it exists now is mostly the top-down, which describes a compliant data catalogue that would work for most general purposes. The bottom-up part involves incorporating different business areas and developing new classes and properties that they need, outputting the model in the format they need for their purposes - ie JSON for an API, or a logical domain profile for a dashboard developer.

When it is complete it will consist of :

- An **enterprise metadata model** (all classes and their properties) with a conceptual and logical view.
- A **domain profile** for each business area (a logical and, where needed or practicable, a physical model of the classes and properties used in that area)
- **Documentation** and, where needed, **instance diagrams** supporting the model and each domain profile

## Latest version

**Updated** - Wednesday 8/7/26  
**Version** - Version 1.6. Erwin model version 41 

## News

Documentation for the dissemination profile is at 1.0, or ready to release.

A new dissemination profile diagram has been created which shows how the model can be resolved into a more traditional entity-relationship shape, ready to feed into a physical model and schema.

The main changes are:
- Slight changes to the Resource Documentation class to allow it to carry access rights and other information
- Model cleaned up and reference to Ontology workstream removed
- Domain profile diagram for dissemination
- Dissemination domain profile updated based on feedback (thank you especially to Laura and Rob)
- Draft instructions for maintaining this repo is in the new documentation/data_architecture directory.
The draft guidance for interpreting the metadata model is available here: [Metadata_Model_Documentation_0.2.docx](https://github.com/ONSdigital/enterprise_metadata_model_updates/raw/refs/heads/main/documentation/Metadata_Model_Documentation_0.2.docx) 

The updated draft domain profile guidance for dissemination is here: [Dissemination_Domain_Profile_Documentation_1.0.docx](https://github.com/ONSdigital/enterprise_metadata_model_updates/raw/refs/heads/main/documentation/domain_profile_dissemination/Dissemination_Domain_Profile_Documentation_1.0.docx). These two documents should be read together.

Instance diagrams and the domain-specific conceptual and logical models for Dissemination are available in the appropriate part of the diagrams directory [here](https://github.com/ONSdigital/enterprise_metadata_model_updates/tree/main/diagrams/dissemination).

Please continue to review the Architecture Decision Records in the [documentation/decisions](documentation/decisions) directory to keep abreast of any recent decisions (nothing important recorded this week, sorry).

## Diagrams

### Conceptual
![V1.6 Conceptual](/diagrams/METADATA_MODEL_CONCEPTUAL_1.6.png)

### Logical
![V1.6 Logical](/diagrams/METADATA_MODEL_LOGICAL_1.6.png)

## Files

Reports and all diagrams are updated for version 1.6.
Dissemination domain profile documentation is also at 1.6.
The documentation for the overall model is at 1.5 but is still valid.

## To do

- Start to firm up the metadata model documentation
- Start to develop a system for managing lineage ([probably using the provenance ontology and data model](https://www.w3.org/TR/2013/NOTE-prov-overview-20130430/))
- [SDMx](https://sdmx.org/) is on the horizon...

## Contact

Message Samantha Iacob on teams or email [samantha.iacob@ons.gov.uk](mailto:samantha.iacob@ons.gov.uk)
I am always happy to discuss ways to improve the model (I would like it to be used so it has to work for you!)

You could also reach out to Kirti Tandel, Hollie Young, Wilfred Inuaghata or Lorraine Crichton for more information. 
