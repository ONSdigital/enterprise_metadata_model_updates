# Model Updates

This is a repository for people to access artifacts around the ONS enterprise-wide **metadata model** and any **metadata profiles** created from it.
This will include reports, documentation, instance diagrams and any other thing useful for understanding the model.
Until a regular cadence for updates is established it will typically be updated on or around Fridays as required.

## Introduction

The ONS metadata model describes an enterprise data catalogue which is based on international standards and identified requirements from business areas that will be interacting with it. To deliver this as quickly as possible it is being built in a top-down and bottom-up way at the same time. The model as it exists now is mostly the top-down, which describes a compliant data catalogue that would work for most general purposes. The bottom-up part involves incorporating different business areas and developing new classes and properties that they need, outputting the model in the format they need for their purposes - ie JSON for an API, or a logical metadata profile for a dashboard developer.

When it is complete it will consist of :

- An **enterprise metadata model** (all classes and their properties) with a conceptual and logical view, and once a cataloguing solution is identified a physical diagram as well.
- A **metadata profile** for each business area that requires it (a logical and, where needed or practicable, a physical model of the classes and properties used in that area)
- **Documentation** and, where needed, **instance diagrams** supporting the model and any metadata profiles

## Latest version

**Updated** - Wednesday 31/7/26  
**Version** - Version 1.7. Erwin model version 55 

## News

Exciting changes - as you may have noticed the repository structure has changed. This is in response to feedback from the business and means that GitHub is able to handle our versioning needs rather than relying on a mix of tables in Word documents.

Major upgrades:
- The documentation is now in markdown, allowing easy comparison between commits.
- The file structure is slightly more logical, with diagrams found near the documents explaining them
- Made the licence for the model explicit with a LICENSE.txt
- Most excitingly, made the repository public in line with ONS Github Usage Policy (since there is nothing sensitive here)

These changes will allow us to decommission the SharePoint mirror, leaving the repository as the single source of truth for the model. On a personal note I won't miss it, updating it was a bit of a bear!

As this situation has become urgent we have begun work on developing a versioning system with an actual update cycle. This will let us manage our workload far more effectively than we have been up until now.

Not to forget the model itself, there have been some slight changes in response to recent feedback and to prepare for developing a Provenance capability. The main one is that the Attribution class relationships have all been made non-identifying and a new identifer has been added for Attribution. References to domain profiles have been stripped out as the nomenclature was incorrect, and for the logical diagrams the colour-coding of classes based on the flavour of W3C-approved standard the class was borrowed from has been removed as it was no longer helpful.

The updated guidance for interpreting the metadata model is available here: [Metadata_Model_Documentation](metadata_model/METADATA_MODEL_DOCUMENTATION.md)

The current metadata profile guidance for dissemination is here: [Dissemination_Metadata_Profile](metadata_profiles/dissemination/DISSEMINATION_METADATA_PROFILE_DOCUMENTATION.md). This document isn't standalone and should be read alongside the metadata model documentation.

Please continue to review the Architecture Decision Records in the [documents/decisions](documents/decisions) directory to keep abreast of any recent decisions.

## Diagrams

### Conceptual
![Conceptual](metadata_model/images/diagrams/METADATA_MODEL_CONCEPTUAL.png)

### Logical
![Logical](metadata_model/images/diagrams/METADATA_MODEL_LOGICAL.png)

## To do

- Incorporate any changes required from the Dissemination metadata profile workstream
- Consider and develop a basic but extensible functionality for risk (using DPV), lineage (Prov) and concept schemes (SKOS)
- Begin to worry at least a little about microdata, as a treat

## Contact

Message Samantha Iacob on teams or email [samantha.iacob@ons.gov.uk](mailto:samantha.iacob@ons.gov.uk)
I am always happy to discuss ways to improve the model!

