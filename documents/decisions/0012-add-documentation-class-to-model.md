# 12. Add Documentation class to model

Date: 12/06/2026 15:01

## Status

ACCEPTED

## Context

The "treat everything as a dataset" approach was something Digital Publishing has been trying to move away from for some time, and documentation is a required class for DORA. It was also expanding the list of dataset types uncomfortably and putting a lot of pressure on the RelatedResouce class to make things work. In short while making (almost) everything catalogued a dataset was simple to model, it was annoying a lot of people and was already creaking. The proposal was to introduce a documentation class.

## Decision

That documentation be a separate class and not a child of the catalogued resources, as documents are not something the catalogue will be managing directly. Rather than gather all the details on them as we would a dataset the class mostly indicates they exist and points to a landing page, which some optional additional properties about creator, date of creation and limited versioning capabilities in case those are needed in some applications.

Wilfred and Sam had a meeting to discuss this and decided to call the class Resource Document as the documentation has no independent existence in the catalogue without its connection to a dataset, series or data service. It was decided that duplication was tolerable (if more than one dataset series has the same quality documentation, it would create a new Resource Documentation instance for each dataset series, all pointing to the same document). This is in line with current practice (basically just pasting a link). 

The Resource Document is of type foaf:document rather than dcat:resource

People involved in this discussion : Charles B, Hollie Y, Lorraine C, Sam I, Wilfred I

## Consequences

This should meet DORA needs, make explaining the documentation model a bit easier, and save on treating documents and other ephemera as full members of the catalogue. 