# 13. Replace Annotation class with Usage Note property in Dataset

Date: 18/06/2026 09:23

## Status

ACCEPTED

## Context

James D Anderson raised the question of whether usage notes and alerts are actually needed. Previous versions of the models had a confusing catch-all class much like the Annotation class was shaping up to be. He proposed at first that annotation should only be for usage notes.

- There are two types of major "annotations" - usage notes/alerts and correction notices.
- Correction notices can be retrieved from the Resource Version Notes property.
- There is significant ambiguity around Usage Note and Alert, with a Usage Note on one set appearing as an Alert on another. The differentiation is how much the person entering the note/alert wants it highlighted on the website. Given this ambiguity James believed it would be better to remove the alert entirely and rely on the Usage Notes.


## Decision

Since the Annotation class would now only hold Usage Notes and could still risk becoming a dumping ground for other bits of information, Sam Iacob proposed removing the class entirely and at least temporarily replacing it with a Usage Note property in Dataset.

## Consequences

Supercedes an earlier decision (0006) to add the "literal" (annotation) class.
- Annotation class removed from the model.
- Alerts will not be possible as currently designed and have been replaced with Usage Note as a property of Dataset (and available to Dataset Series) which will cover the combined use cases of alerts and usage notes.
- Correction Notices will be drawn from Version Notes
- The domain-specific documentation is to be updated with this information