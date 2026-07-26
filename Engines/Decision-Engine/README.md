# Decision Engine

## Purpose

Serve as the central decision layer for the SOC Central System. The Decision Engine receives approved recommendations from other engines and determines the best next action according to `Architecture/Business-Principles.md`.

## Business Goal

Make system decisions consistent, evidence-backed, explainable, safe, and easy for a human reviewer to approve or override.

## Inputs

* Approved recommendations from business engines
* Authoritative prospect or customer record
* Current approved customer-journey stage
* Supporting evidence and confidence
* Suppression, safety, and human-review status
* Approved business and decision rules

## Outputs

* Recommended next action or no action
* Selected approved opportunity, property, image, journey step, or video when applicable
* Supporting evidence
* Applied rules and Business Principles
* Explanation and confidence
* Human-review requirement
* Decision status and audit details

## Example Decisions

* Which personalization opportunity to use
* Which featured property to display
* Which approved image to use
* Which customer journey step comes next
* Which approved video should be presented
* Whether human review is required
* Whether no action should be taken

## Boundaries

* Never invent facts.
* Never override suppression or safety rules.
* Follow `Architecture/Business-Principles.md`.
* Every decision must have supporting evidence.
* Every decision must be explainable.
* Human approval overrides AI recommendations.
* Do not generate or send outbound communication.
* Do not scrape, connect to live integrations, or build production automation.
* Do not change the approved customer journey.

## Design Documents

* `Decision-Principles.md` — Governing priorities and safeguards.
* `Decision-Workflow.md` — Decision stages and human-review outcomes.
* `Decision-Rules.md` — Rule precedence, eligibility, selection, and no-action rules.
* `Decision-Data-Flow.md` — Central input, decision, output, and exception paths.
* `Decision-Examples.md` — Reviewable examples of supported decisions.

## Current Status

**Design only.** No decision automation, outbound communication, scraping, or live integration has been created.

## Next Approval Required

June must approve the principles, workflow, rules, data flow, and examples before implementation begins.
