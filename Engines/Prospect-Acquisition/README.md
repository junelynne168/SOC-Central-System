# Prospect Acquisition Engine

## Purpose

Identify suitable Realtor prospects, collect reliable public business information, prevent duplicates, and prepare evidence-backed prospect records for human review before any First Impression Email is sent.

## Business Goal

Improve the quality and consistency of prospect selection while reducing repetitive research and protecting June’s time for valuable review and customer conversations.

## Inputs

* Provisionally approved prospect criteria
* Permitted public business sources
* Existing authoritative prospect and customer records
* Suppression and do-not-contact status
* Human-review and automation rules

## Outputs

* Candidate records with source evidence
* Duplicate and validation results
* Proposed prospect scores with explanations
* Approved, rejected, deferred, or incomplete review outcomes
* Approved prospect records ready to move to the First Impression Engine

## Boundaries

* Design suitable Realtor prospect acquisition before automation.
* Use only approved public business information and preserve source evidence.
* Do not invent missing information, permission, APIs, credentials, or legal conclusions.
* Do not automatically merge records.
* Do not contact prospects or send First Impression Emails.
* Human review is required before a prospect advances.
* An approved prospect outcome does not itself authorize contact.

## Design Documents

* `Prospect-Criteria.md` — Provisional target, qualification, and exclusion criteria.
* `Prospect-Sources.md` — Public-source placeholders, concerns, permitted-use checks, and verification.
* `Prospect-Scoring.md` — Proposed 100-point prioritization framework.
* `Prospect-Review-Workflow.md` — Human-review stages, evidence, and outcomes.
* `Duplicate-Prevention.md` — Matching fields, result levels, and review safeguards.
* `Prospect-Acquisition-Data-Flow.md` — Primary flow and exception paths.

## Current Status

**Design only.** No scraping, live-source connection, communication, or production automation has been created.

## Next Approval Required

June must approve the criteria, sources, scoring framework, review workflow, duplicate rules, and data flow before implementation begins.
