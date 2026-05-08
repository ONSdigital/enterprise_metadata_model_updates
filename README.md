# Model Updates

This is a repository for people to access artifacts around the EMM enterprise **metadata model** and any **domain profiles** created from it.
This will include reports, documentation, instance diagrams and any other thing useful for understanding the model.
It will be updated at least weekly (probably on Fridays) until it reaches a more settled state.

Please watch this repo for updates or come back next Friday :)

## Introduction

The ONS metadata model describes an enterprise data catalogue which is based on international standards and identified requirements from business areas that will be interacting with it. To deliver this as quickly as possible it is being built in a top-down and bottom-up way at the same time. The model as it exists now is mostly the top-down, which describes a compliant data catalogue that would work for most general purposes. The bottom-up part involves incorporating different business areas and developing new classes and properties that they need, outputting the model in the format they need for their purposes - ie JSON for an API, or a logical domain profile for a dashboard developer.

When it is complete it will consist of :

- An **enterprise metadata model** (all classes and their properties) with a conceptual and logical view.
- A **domain profile** for each business area (a logical and, where needed or practicable, a physical model of the classes and properties used in that area)
- **Documentation** and **instance diagrams** supporting each domain profile

## Latest version

**Updated** - Fri 8/5/26  
**Version** - Version 1.2 . Erwin model version 21 

## News

New classes to support DORA/DS-DP requirements have been added to the model (specifically Literal, Variable and Frequency classes). See the [Entity Definitions report](/reports/Entity_Definitions_1.2.csv) for more details.

A legend has been added to the Logical Diagram.

**Architectural Decision Record** is updated. As of 8/5 the current decisions are outstanding (mostly I've already put them in the model but it would be good to review those changes). Have a look in the [documentation/decisions](documentation/decisions) directory for more information.

New decisions are decisions 4-7. The proposed decisions are:

- ***5**: [Add Resource Next Version ID to Resource class](documentation/decisions/0005-add-resource-next-version-id-to-resource-class.md)*
- ***6**: [Add Literal class to handled Alerts](documentation/decisions/0006-add-literal-class-to-handle-alerts.md)*


## Diagrams

### Conceptual
![V1.2 Conceptual](/diagrams/METADATA_MODEL_CONCEPTUAL_V1.2.PNG)

### Logical
![V1.2 Logical](/diagrams/METADATA_MODEL_LOGICAL_V1.2.PNG)

### Physical

*(JSON architecture)*
![V1.2 Physical](/diagrams/METADATA_MODEL_PHYSICAL_V1.2.PNG)


## Files

Reports and json directories are updated for version 1.2.

## To do

- Dissemination domain profile and JSON for DS-DP.
- DORA profile and JSON
- Improve the format of this repo

## Contact

Message Samantha Iacob on teams or email [samantha.iacob@ons.gov.uk](mailto:samantha.iacob@ons.gov.uk)
I am always happy to discuss ways to improve the model (I would like it to be used so it has to work for you!)
