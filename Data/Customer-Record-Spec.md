# Customer Record Specification

## Purpose

Define the minimum authoritative record after a prospect becomes a customer.

## Proposed Fields

- Customer identifier
- Linked prospect identifier
- Name
- Approved contact information
- Customer confirmation and start date
- Current relationship stage
- Journey and stage history
- Onboarding outcomes
- Communication preferences and permissions
- Relationship context with source evidence
- Follow-up history references
- Assigned next action
- Exception or human-review status
- Created and last-modified timestamps

## Rules

- Convert or link the existing prospect record; do not create an unrelated duplicate.
- Preserve prospect and onboarding history.
- Store only approved relationship context.
- Respect communication preferences and suppression decisions.
- Define detailed field types and required values before automation begins.
