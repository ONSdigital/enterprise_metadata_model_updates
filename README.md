# Model Updates

This is a repository for people to access artifacts around the EMM enterprise **metadata model** and any **domain profiles** created from it.
This will include reports, documentation, instance diagrams and any other thing useful for understanding the model.
It will be updated at least weekly (probably on Fridays) until it reaches a more settled state.

## Introduction

The ONS metadata model describes an enterprise data catalogue which is based on international standards and identified requirements from business areas that will be interacting with it. To deliver this as quickly as possible it is being built in a top-down and bottom-up way at the same time. The model as it exists now is mostly the top-down, which describes a compliant data catalogue that would work for most general purposes. The bottom-up part involves incorporating different business areas and developing new classes and properties that they need, outputting the model in the format they need for their purposes - ie JSON for an API, or a logical domain profile for a dashboard developer.

When it is complete it will consist of :

- An **enterprise metadata model** (all classes and their properties) with a conceptual and logical view.
- A **domain profile** for each business area (a logical and, where needed or practicable, a physical model of the classes and properties used in that area)
- **Documentation** and **instance diagrams** supporting each domain profile

## Latest version

**Updated** - Fri 1/5/26  
**Version** - Version 1.1 . Erwin model version 15 

## News

Architectural Decision Record has been implemented - all major changes to this model and the reasons for those changes can be found in [documentation/decisions](/documentation/decisions).

Check the reports folder for entity and logical/physical attribute definitions in the current model.

The biggest changes this update are changes to attribute names to remove references to "codes" (as this was confusing) and the addition of the Catalogue Resource class to track when entries in the catalogue are created or changed, as opposed to the actual datasets themselves.


## Diagrams

### Conceptual
![V1.1 Conceptual](/diagrams/METADATA_MODEL_CONCEPTUAL_V1.1.PNG)

### Logical
![V1.1 Logical](/diagrams/METADATA_MODEL_LOGICAL_V1.1.PNG)

### Physical

*(JSON architecture)*
![V1.1 Physical](/diagrams/METADATA_MODEL_PHYSICAL_V1.1.PNG)


## Files

Reports and json directories are updated for version 1.1.

## To do

- Integrate DS-DP requirements and metadata attributes (thank you Lorraine and Hollie)
- Integrate DORA and expand the model to incorporate table- and variable-level metadata.
- Create a DS-DP domain profile and instance models.
- Improve the JSON
- Improve the format of this repo

## Contact

Message Samantha Iacob on teams or email [samantha.iacob@ons.gov.uk](mailto:samantha.iacob@ons.gov.uk)
I am always happy to discuss ways to improve the model (I would like it to be used so it has to work for you!)
