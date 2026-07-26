# Decision Rules

## Purpose

Define a simple rule order for selecting the best next action without bypassing evidence, safety, human review, or the approved customer journey.

## Rule Precedence

Apply rules in this order:

1. Human-approved instruction
2. Suppression and safety rules
3. Required approval and eligibility rules
4. Approved customer-journey rules
5. `Architecture/Business-Principles.md`
6. Evidence strength and confidence
7. Lowest customer effort
8. Simplest reliable next action
9. AI recommendation ranking

A lower rule may never override a higher rule.

## Eligibility Rules

An action is eligible only when:

* It is allowed for the current journey stage.
* Required facts and recommendations are approved.
* Supporting evidence is available.
* Suppression and safety checks permit consideration.
* Required assets, links, or videos are approved.
* Required human review is complete or is explicitly the next action.

## Selection Rules

When more than one action is eligible:

1. Prefer the action that fits the current approved journey step.
2. Prefer the action that gives the customer one clear next action.
3. Prefer lower customer effort and lower technical complexity.
4. Prefer stronger, more recent, and more relevant evidence.
5. Prefer the action that preserves June’s attention for valuable conversations.
6. Prefer the simplest reliable action.
7. Require human review when the remaining choice is uncertain or sensitive.

## Decision-Type Rules

### Personalization Opportunity

Choose only from human-approved intelligence recommendations. Preserve the evidence, confidence, and reviewer limitations.

### Featured Property

Choose only an approved property clearly tied to the prospect and selected personalization opportunity.

### Approved Image

Choose only an approved image whose source, subject, intended use, and relationship to the opportunity are verified.

### Customer Journey Step

Choose only the next permitted step from the approved seven-step journey. Do not skip, insert, or reorder steps without June’s approval.

### Approved Video

Choose the approved video assigned to the current journey need. The 3-minute iPhone demonstration remains primary; the 7-minute computer tutorial is optional for people who prefer a computer.

### Human Review

Require review whenever policy, uncertainty, sensitivity, conflict, or missing approval requires it.

### No Action

Choose no action when no option is eligible, evidence is inadequate, suppression applies, safety is unresolved, timing is inappropriate, or action would add unnecessary customer effort.

## Conflict Rule

If approved rules conflict or the correct precedence is uncertain, stop and require human review. Do not guess.
