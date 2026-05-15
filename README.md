# Model Updates

This is a repository for people to access artifacts around the EMM enterprise **metadata model** and any **domain profiles** created from it.
This will include reports, documentation, instance diagrams and any other thing useful for understanding the model.
It will be updated at least weekly (probably on Fridays) until it reaches a more settled state.

Please watch this repo for updates or come back next Friday :)

The models and reviews are (at least temporarily) [mirrored on ONS SharePoint](https://officenationalstatistics.sharepoint.com/sites/Metadata/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FMetadata%2FShared%20Documents%2F1%2E%20Enterprise%20Metadata%20Management%20%28EMM%29%2FEMM%20Workstreams%2FONS%20Metadata%20Model&viewid=22b51cd2%2D15c6%2D4d18%2Dbc10%2Dbc9e433ec574&newTargetListUrl=%2Fsites%2FMetadata%2FShared%20Documents&viewpath=%2Fsites%2FMetadata%2FShared%20Documents%2FForms%2FAllItems%2Easpx) if you need to share with anyone who doesn't have an ONS Digital account. [🔗Link](https://officenationalstatistics.sharepoint.com/sites/Metadata/Shared%20Documents/Forms/AllItems.aspx?id=%2Fsites%2FMetadata%2FShared%20Documents%2F1%2E%20Enterprise%20Metadata%20Management%20%28EMM%29%2FEMM%20Workstreams%2FONS%20Metadata%20Model&viewid=22b51cd2%2D15c6%2D4d18%2Dbc10%2Dbc9e433ec574&newTargetListUrl=%2Fsites%2FMetadata%2FShared%20Documents&viewpath=%2Fsites%2FMetadata%2FShared%20Documents%2FForms%2FAllItems%2Easpx)

## Introduction

The ONS metadata model describes an enterprise data catalogue which is based on international standards and identified requirements from business areas that will be interacting with it. To deliver this as quickly as possible it is being built in a top-down and bottom-up way at the same time. The model as it exists now is mostly the top-down, which describes a compliant data catalogue that would work for most general purposes. The bottom-up part involves incorporating different business areas and developing new classes and properties that they need, outputting the model in the format they need for their purposes - ie JSON for an API, or a logical domain profile for a dashboard developer.

When it is complete it will consist of :

- An **enterprise metadata model** (all classes and their properties) with a conceptual and logical view.
- A **domain profile** for each business area (a logical and, where needed or practicable, a physical model of the classes and properties used in that area)
- **Documentation** and **instance diagrams** supporting each domain profile

## Latest version

**Updated** - Fri 15/5/26  
**Version** - Version 1.3 . Erwin model version 22 

## News

Following some careful digging, instance diagramming and lots and lots of in-depth discussions (thank you Wilfred, Lorraine, Charles, Kirti, Tanita, Hollie, Laura and Rob especially) the metadata model now covers the required properties for dissemination/digital publishing. 

Said instance diagram is available in [diagrams/dissemination](https://github.com/ONSdigital/enterprise_metadata_model_updates/tree/main/diagrams/dissemination)

Physical diagrams and reports have, for now, been removed as there's no need for an "overall" metadata model schema and they don't reveal anything the logical models and reports don't already cover. These will reappear in domain profiles as they near completion.

**Architectural Decision Record** continues to be updated. Have a look in the [documentation/decisions](documentation/decisions) directory to review any recent decisions.

## Diagrams

### Conceptual
![V1.3 Conceptual](/diagrams/METADATA_MODEL_CONCEPTUAL_V1.3.PNG)

### Logical
![V1.3 Logical](/diagrams/METADATA_MODEL_LOGICAL_V1.3.PNG)

## Files

Reports are updated for version 1.3. The json reflects version 1.2 but is in line for an update shortly (it will also move to the appropriate domain profiles).

## To do

- Dissemination domain profile due next week.
- DORA profile being worked on by the rest of the team

## Contact

Message Samantha Iacob on teams or email [samantha.iacob@ons.gov.uk](mailto:samantha.iacob@ons.gov.uk)
I am always happy to discuss ways to improve the model (I would like it to be used so it has to work for you!)
