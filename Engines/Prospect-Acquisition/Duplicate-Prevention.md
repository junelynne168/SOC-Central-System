# Duplicate Prevention

## Purpose

Prevent duplicate prospect and customer records before a candidate advances to human review or the First Impression Engine.

## Matching Fields

Compare available, normalized values for:

* Public business email
* Phone number
* Website
* Full name plus brokerage
* Full name plus market location
* Existing prospect identifier
* Existing customer identifier

Normalization may support comparison, but the original source values and evidence must be preserved.

## Match Results

### Exact Match

One or more reliable unique identifiers match exactly, or the evidence clearly identifies the same authoritative record. Do not create or advance a duplicate record.

### Probable Match

Multiple strong fields match, but identity is not conclusive. Human review is required.

### Possible Match

One or more non-unique or incomplete fields suggest the same person. Human review is required.

### No Match

No meaningful match is found using the available approved fields. This result permits the workflow to continue but does not guarantee uniqueness.

## Rules

* Probable and possible matches require human review.
* Do not automatically merge records.
* Do not overwrite existing prospect or customer information.
* Existing customer status, prior contact, and suppression status must be checked before advancement.
* Record the fields compared, result, candidate records, evidence, reviewer decision, and timestamp.
* When identity remains uncertain, stop and mark the candidate incomplete or deferred.
