# 22. Change version system from semantic to date based

Date: 04/08/2026 14:38

## Status

ACCEPTED

## Context

The current versioning system is a semantic one,  x.y.z (1.15.2 for instance)

x is a major version which includes an entirely new system or major changes to the classes and how they interact which breaks compatibility with previous models
y is a minor version which might include new classes, properties and relationships but which does not radically change how the overall system works 
z is a correction where a minor error is fixed (for instance spelling errors, a relationship line accidentally set as identifying when it should be non-identifying if you get to it quickly enough

This system is useful for aligning things - so if diagrams and documents have the same version number they are aligned.
Problem : the difference between x and y is arbitrary and sometimes y will go up for very major or minor things (replacing the document model was one of these big changes a couple of minor versions ago). The semantic numbering system has no business meaning, or any meaning at all - you have to go look at another file like the github readme for more info and hope Sam put it there. As different bits of the business develop systems off of a particular version of the model, they will slip out of line with overall development really easily and have to go digging around for say the metadata documentation that aligns to whatever model version they're building off. It is fiddly and difficult to deal with.

Since the model is provided through GitHub it's easier for users just to note the date of the commit they want to reference. All files on the repo are aligned at the time a commit is made and the whole repo can be rolled back to any commit a user needs (and as of the last update it will also meaningfully highlight what's changed between the two versions). As Sam I is bad at GitHub and will make multiple commits on a single day to correct spelling errors or broken links it would be preferable to have a version system that refers to the last commit made on that date and you could refer to the model at a certain point by the date alone. Business people could then say things like "I would like KIM integrated into this model by 31 October" and then they will know that the 31 Oct commit should contain what they asked for. We can also say things like "expect this feature in the 31 November update" instead which will make more sense than saying "it's coming in version 2.9".

In short Sam thinks it's easier to manage this system, it's less confusing for everyone and there's no real downside to switching over except for spreadsheet fans who will have one less spreadsheet to manage.


## Decision

This was accepted in late August and the version system simply reflects the date of the GitHub commit to main.

## Consequences

This will cause some issues with existing strategic planning around version numbers but unlikely to cause much confusion in the long term.