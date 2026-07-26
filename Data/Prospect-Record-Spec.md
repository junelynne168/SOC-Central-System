# Prospect Record Specification

## Purpose

Define the minimum authoritative record for a person before customer conversion.

## Proposed Fields

- Prospect identifier
- Name
- Organization or business context
- Approved contact information
- Source and source timestamp
- Prospect-review status
- Current journey stage
- Stage history
- Contact approval and suppression status
- Communication history references
- Engagement evidence
- Assigned next action
- Exception or human-review status
- Created and last-modified timestamps

## Rules

- Use one prospect record across all engines.
- Store source evidence for material facts.
- Do not invent missing personal or contact data.
- Record consent, suppression, and review decisions where applicable.
- Define detailed field types and required values before automation begins.
