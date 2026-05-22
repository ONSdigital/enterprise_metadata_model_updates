# Model Updates

This is a repository for people to access artifacts around the ONS enterprise-wide **metadata model** and any **domain profiles** created from it.
This will include reports, documentation, instance diagrams and any other thing useful for understanding the model.
It will be updated weekly on Fridays until it reaches a more settled state.

Please watch this repo for updates or come back around the 12th of June :)

The models and reviews are (at least temporarily) [mirrored on ONS SharePoint](https://officenationalstatistics.sharepoint.com/sites/Metadata/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FMetadata%2FShared%20Documents%2F1%2E%20Enterprise%20Metadata%20Management%20%28EMM%29%2FEMM%20Workstreams%2FONS%20Metadata%20Model&viewid=22b51cd2%2D15c6%2D4d18%2Dbc10%2Dbc9e433ec574&newTargetListUrl=%2Fsites%2FMetadata%2FShared%20Documents&viewpath=%2Fsites%2FMetadata%2FShared%20Documents%2FForms%2FAllItems%2Easpx) if you need to share with anyone who doesn't have an ONS Digital account. [🔗Link](https://officenationalstatistics.sharepoint.com/sites/Metadata/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FMetadata%2FShared%20Documents%2F1%2E%20Enterprise%20Metadata%20Management%20%28EMM%29%2FEMM%20Workstreams%2FONS%20Metadata%20Model&viewid=22b51cd2%2D15c6%2D4d18%2Dbc10%2Dbc9e433ec574&newTargetListUrl=%2Fsites%2FMetadata%2FShared%20Documents&viewpath=%2Fsites%2FMetadata%2FShared%20Documents%2FForms%2FAllItems%2Easpx)

## Introduction

The ONS metadata model describes an enterprise data catalogue which is based on international standards and identified requirements from business areas that will be interacting with it. To deliver this as quickly as possible it is being built in a top-down and bottom-up way at the same time. The model as it exists now is mostly the top-down, which describes a compliant data catalogue that would work for most general purposes. The bottom-up part involves incorporating different business areas and developing new classes and properties that they need, outputting the model in the format they need for their purposes - ie JSON for an API, or a logical domain profile for a dashboard developer.

When it is complete it will consist of :

- An **enterprise metadata model** (all classes and their properties) with a conceptual and logical view.
- A **domain profile** for each business area (a logical and, where needed or practicable, a physical model of the classes and properties used in that area)
- **Documentation** and **instance diagrams** supporting each domain profile

## Latest version

**Updated** - Fri 22/5/26  
**Version** - Version 1.4. Erwin model version 28 

## News

Draft guidance for interpreting the metadata model is available! Download it here: [Metadata_Model_Documentation_0.1.docx](https://github.com/ONSdigital/enterprise_metadata_model_updates/raw/refs/heads/main/documentation/Metadata_Model_Documentation_0.1.docx)  

The first domain profile guidance is out too, for DS-DP. It's designed to be read together with the Metadata Model Documentation. Download it here: [DS-DP_Domain_Profile_Documentation_0.1.docx](https://github.com/ONSdigital/enterprise_metadata_model_updates/raw/refs/heads/main/documentation/domain_profile_DS_DP/DS-DP_Domain_Profile_Documentation_0.1.docx) 

New instance diagrams and the domain-specific conceptual and logical models for DS-DP are now available in the appropriate part of the diagrams directory [here](https://github.com/ONSdigital/enterprise_metadata_model_updates/tree/main/diagrams/ds-dp).

These documents and resources are in an early state of development and feedback will be very gratefully received. 

Please continue to review the Architecture Decision Records in the [documentation/decisions](documentation/decisions) directory to keep abreast of any recent decisions.

## Diagrams

### Conceptual
![V1.4 Conceptual](/diagrams/METADATA_MODEL_CONCEPTUAL_1.4.PNG)

### Logical
![V1.4 Logical](/diagrams/METADATA_MODEL_LOGICAL_1.4.PNG)

## Files

Reports are updated for version 1.4. The JSON has been removed as it is a few versions outdated and not relevant at the overall model level. It will reappear in the domain profiles as it is completed for each area.

## To do

- I (Samantha) am going on vacation for two weeks and not thinking about metadata. This repository is unlikely to see any updates before I return.
- The DAB team is continuing to develop the DORA and DS-DP domain profiles and overall metadata model design
- When I return I plan to improve the documentation based on feedback I receive

## Contact

Message Samantha Iacob on teams or email [samantha.iacob@ons.gov.uk](mailto:samantha.iacob@ons.gov.uk)
I am always happy to discuss ways to improve the model (I would like it to be used so it has to work for you!)

While I am away (or even when I'm here) please contact Kirti Tandel or Hollie Young to discuss everything metadata model.
