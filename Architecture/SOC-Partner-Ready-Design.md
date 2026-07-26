# SOC Partner-Ready Design

## Purpose

Define how the SOC Central System can remain simple for June’s business while also being shared with partners and offered to other partners within the SOC organization.

## Primary Rule

This system is designed specifically for the SOC business.

Possible future use in other industries may be remembered, but it must not add complexity to the current SOC design.

## Simplicity Requirements

* Use clear business language.
* Avoid unnecessary technical terminology.
* Keep each workflow short and visible.
* Give the user one clear next action.
* Use one authoritative prospect and customer record.
* Avoid duplicate engines, records, settings, and reports.
* Prefer configuration over custom redevelopment.
* Require as little manual work as reasonably possible.
* Keep human review only where it protects quality, safety, or important relationships.

## Partner-Ready Requirements

A partner should be able to configure:

* Partner name
* Business name
* Contact information
* Service area
* Email signature
* Appointment link
* Online sign-up link
* SOC card-creation link
* Approved video links
* Branding assets
* Sending limits
* Human-review preferences

These settings must be separated from the core system logic.

## Shared Core

All SOC partners should use the same approved core:

* Prospect Acquisition
* Prospect Intelligence
* Decision Engine
* First Impression
* Customer Journey
* Customer Onboarding
* Relationship Generator
* AI Video Production
* Safety and review rules
* Prospect and customer data structure

## Partner Configuration

Partner-specific information should be stored in one configuration area rather than rewritten throughout the system.

No partner should need to edit engine logic for ordinary setup.

## Distribution Principle

The system should eventually support a repeatable process:

SOC Core System
→ Add Partner Configuration
→ Test
→ Approve
→ Launch for Partner

## Boundaries

* Do not build a multi-industry platform now.
* Do not add insurance, mortgage, financial-advisor, or other industry workflows.
* Do not add complicated multi-tenant technology during the current design phase.
* Do not sacrifice the simplicity of June’s SOC system for hypothetical future use.
* Do not create production deployment automation yet.

## Design Review Questions

Before adding anything, ask:

1. Is this necessary for the SOC business?
2. Will June and her partner understand it?
3. Can another SOC partner configure it easily?
4. Does it reduce rather than increase manual work?
5. Can the same goal be achieved more simply?

If not, simplify or reject it.
