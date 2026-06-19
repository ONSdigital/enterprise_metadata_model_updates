# Model Updates

This is a repository for people to access artifacts around the ONS enterprise-wide **metadata model** and any **domain profiles** created from it.
This will include reports, documentation, instance diagrams and any other thing useful for understanding the model.
It will typically be updated on Fridays.

The next update is expected by Friday 26 June.

The models and reviews are (at least temporarily) [mirrored on ONS SharePoint](https://officenationalstatistics.sharepoint.com/sites/Metadata/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FMetadata%2FShared%20Documents%2F1%2E%20Enterprise%20Metadata%20Management%20%28EMM%29%2FEMM%20Workstreams%2FONS%20Metadata%20Model&viewid=22b51cd2%2D15c6%2D4d18%2Dbc10%2Dbc9e433ec574&newTargetListUrl=%2Fsites%2FMetadata%2FShared%20Documents&viewpath=%2Fsites%2FMetadata%2FShared%20Documents%2FForms%2FAllItems%2Easpx) if you need to share with anyone who doesn't have an ONS Digital account. [🔗Link](https://officenationalstatistics.sharepoint.com/sites/Metadata/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FMetadata%2FShared%20Documents%2F1%2E%20Enterprise%20Metadata%20Management%20%28EMM%29%2FEMM%20Workstreams%2FONS%20Metadata%20Model&viewid=22b51cd2%2D15c6%2D4d18%2Dbc10%2Dbc9e433ec574&newTargetListUrl=%2Fsites%2FMetadata%2FShared%20Documents&viewpath=%2Fsites%2FMetadata%2FShared%20Documents%2FForms%2FAllItems%2Easpx)

## Introduction

The ONS metadata model describes an enterprise data catalogue which is based on international standards and identified requirements from business areas that will be interacting with it. To deliver this as quickly as possible it is being built in a top-down and bottom-up way at the same time. The model as it exists now is mostly the top-down, which describes a compliant data catalogue that would work for most general purposes. The bottom-up part involves incorporating different business areas and developing new classes and properties that they need, outputting the model in the format they need for their purposes - ie JSON for an API, or a logical domain profile for a dashboard developer.

When it is complete it will consist of :

- An **enterprise metadata model** (all classes and their properties) with a conceptual and logical view.
- A **domain profile** for each business area (a logical and, where needed or practicable, a physical model of the classes and properties used in that area)
- **Documentation** and **instance diagrams** supporting each domain profile

## Latest version

**Updated** - Fri 19/6/26  
**Version** - Version 1.5. Erwin model version 31 

## News

This is a technical update which only includes the models and reports, supporting documentation will be updated over the next week.

The main changes are:
- A new **Resource Documentation** class - you don't have to create docs as a dataset anymore which should make life easier.
- Removed the **Annotation** class due to the risk of having a kind of "dump" class for notes and things and some ambiguity about what kind of messages go in there, and why. It has been absorbed into the already existing _Version Note_ and the new _Usage Note_ properties.
- Removed **Variable** as it is not currently required by any stakeholders. Schema and variable-level metadata is important and complex to model, and it touches on a lot of business areas, so we will take the time to get it right.
- Renamed DS-DP things to Dissemination to reflect the GSBPM stage the catalogue is working with. A minor change now but this will help everyone sing from the same hymn sheet later on.
- Physical diagram removed entirely from the ONS metadata model. It wasn't being updated or published here and it wasn't helpful to maintain it for the time being. Physical diagrams belong with their domain profiles and will be released as they're completed.

Draft guidance for interpreting the metadata model is available! Download it here: [Metadata_Model_Documentation_0.1.docx](https://github.com/ONSdigital/enterprise_metadata_model_updates/raw/refs/heads/main/documentation/Metadata_Model_Documentation_0.1.docx) This is currently in line with version 1.4 and will be updated over the next week. 

The first domain profile guidance is out too, for DS-DP. It's designed to be read together with the Metadata Model Documentation. Download it here: [DS-DP_Domain_Profile_Documentation_0.1.docx](https://github.com/ONSdigital/enterprise_metadata_model_updates/raw/refs/heads/main/documentation/domain_profile_DS_DP/DS-DP_Domain_Profile_Documentation_0.1.docx). Likewise this is slightly outdated given the new model and will be updated.

Instance diagrams and the domain-specific conceptual and logical models for DS-DP are now available in the appropriate part of the diagrams directory [here](https://github.com/ONSdigital/enterprise_metadata_model_updates/tree/main/diagrams/ds-dp).

These documents and resources are in an early state of development and feedback will be very gratefully received. 

Please continue to review the Architecture Decision Records in the [documentation/decisions](documentation/decisions) directory to keep abreast of any recent decisions.

## Diagrams

### Conceptual
![V1.5 Conceptual](/diagrams/METADATA_MODEL_CONCEPTUAL_1.5.PNG)

### Logical
![V1.5 Logical](/diagrams/METADATA_MODEL_LOGICAL_1.5.PNG)

## Files

Reports are updated for version 1.5. 

## To do

- Bring the documentation for the overall model and the dissemination profile in line with the diagrams. This is due by 26 June.
- Instructions for updating the repository will allow EMM project members to contribute to this repository.
- Version 2 will focus on incorporating the DORA (process phase) domain profile into the model.
- As the model is formally adopted, changing it will have implications across the business. Updates will therefore slow down and begin to follow a more predictable cycle (the form this cycle will take is not yet decided)

## Contact

Message Samantha Iacob on teams or email [samantha.iacob@ons.gov.uk](mailto:samantha.iacob@ons.gov.uk)
I am always happy to discuss ways to improve the model (I would like it to be used so it has to work for you!)

You could also reach out to Kirti Tandel, Hollie Young, Wilfred Inuaghata or Lorraine Crichton for more information. 
