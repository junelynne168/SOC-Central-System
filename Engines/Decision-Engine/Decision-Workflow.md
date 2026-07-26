# Decision Workflow

## Workflow

1. Approved recommendation package received
2. Authoritative record and current journey stage confirmed
3. Suppression and safety gates checked
4. Evidence and approval status validated
5. Eligible actions identified
6. Business Principles and decision rules applied
7. Best next action or no action recommended
8. Explanation, evidence, confidence, and review requirement recorded
9. Human review performed when required
10. Approved decision returned to the appropriate business engine

## Required Decision Record

* Decision identifier
* Prospect or customer identifier
* Source engine
* Current journey stage
* Candidate actions considered
* Selected action or no action
* Supporting evidence
* Rules and Business Principles applied
* Confidence and known limitations
* Suppression and safety result
* Human-review requirement
* Reviewer decision and reason when applicable
* Destination business engine
* Created and reviewed timestamps

## Decision Outcomes

### Approved

A human reviewer approves the recommended action for return to the appropriate engine. Approval does not independently authorize outbound sending.

### Replaced

A human reviewer selects a different eligible action and records the supporting reason and evidence.

### Rejected

The proposed action must not proceed. Record the reason.

### Deferred

No action should occur until an approved time, condition, or evidence requirement is met.

### No Action

The evidence, safety status, journey fit, or business value does not justify an action.

### Incomplete

Required evidence, approval, or authoritative record information is missing or contradictory.

## Human Review Triggers

Human review is required when:

* A suppression or safety status is unresolved.
* Evidence is contradictory, incomplete, or low confidence.
* Multiple options remain equally suitable.
* A sensitive customer-facing decision is involved.
* Another engine marks the recommendation for review.
* An exception or rule conflict exists.
* Approved policy explicitly requires review.

## Handoff Rule

Return only an approved decision package. The receiving engine remains responsible for its own approved workflow and communication controls.
