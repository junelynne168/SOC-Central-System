# System Architecture

## Purpose

Define the seven connected business engines and the central Decision Engine that support the SOC customer journey. This is an architecture foundation only; production automations are not yet authorized.

## Business Principles

All engines, integrations, automations, and customer experiences must follow `Business-Principles.md`.

## SOC Scope and Partner Reuse

* The architecture remains SOC-specific.
* All partners share the same core engine design.
* Partner information is configuration, not separate engine logic.
* Multi-industry platform design is outside the current scope.

## Central Decision Layer

### Decision Engine

- Purpose: Receive approved recommendations from business engines and determine the best next action according to `Business-Principles.md`.
- Inputs: Approved recommendations, authoritative record and journey stage, supporting evidence, confidence, suppression and safety status, and human-review status.
- Outputs: Explainable recommended action or no action, supporting evidence, applied rules, and human-review requirement.
- Connects to: Prospect Acquisition Engine, Prospect Intelligence Engine, First Impression Engine, Customer Journey Engine, Customer Onboarding Engine, Relationship Generator Engine, and AI Video Production System.
- Boundaries: Never invent facts, override suppression or safety rules, change the approved journey, generate outbound communication, or overrule a human approval.

## Engines

### 1. Prospect Acquisition Engine

- Purpose: Find and organize suitable prospects for review.
- Inputs: Prospect criteria and permitted prospect-source information.
- Outputs: Approved prospect records with source, score, duplicate, suppression, and review evidence.
- Connects to: Prospect Intelligence Engine and the shared prospect record.

### 2. Prospect Intelligence Engine

- Purpose: Transform approved prospect records into meaningful, evidence-backed personalization recommendations.
- Inputs: Approved prospect record, verified source evidence, score explanation, and review status.
- Outputs: Human-reviewed personalization recommendation, confidence level, and supporting evidence.
- Connects to: Prospect Acquisition Engine, First Impression Engine, and the shared prospect record.

### 3. First Impression Engine

- Purpose: Create a relevant, personalized first impression.
- Inputs: Approved prospect record, human-approved intelligence package, approved messaging, and approved communication assets.
- Outputs: Approved First Impression Email and engagement signals.
- Connects to: Prospect Intelligence Engine, Customer Journey Engine, and human review.

### 4. Customer Journey Engine

- Purpose: Guide each person through the approved seven-step journey.
- Inputs: Prospect or customer stage, engagement signals, and approved next actions.
- Outputs: Journey-stage updates and the next approved action.
- Connects to: First Impression, Customer Onboarding, Relationship Generator, and shared records.

### 5. Customer Onboarding Engine

- Purpose: Help an engaged prospect create and send a first free card, then choose sign-up or personal help.
- Inputs: Engaged prospect record, approved demonstrations, and card-creation access.
- Outputs: Free Card User, Qualified Lead, or Customer status and onboarding outcomes.
- Connects to: Customer Journey Engine, AI Video Production System, scheduling, and online sign-up.

### 6. Relationship Generator Engine

- Purpose: Support meaningful long-term relationship marketing after onboarding.
- Inputs: Approved customer record, relationship context, milestones, and communication rules.
- Outputs: Human-reviewed relationship and follow-up opportunities.
- Connects to: Customer Journey Engine and the shared customer record.

### 7. AI Video Production System

- Purpose: Produce and maintain approved video guidance used throughout the journey.
- Inputs: Approved scripts, demonstrations, brand requirements, and review decisions.
- Outputs: Approved 30-second introduction, 3-minute iPhone demonstration, optional 7-minute computer tutorial, and future approved videos.
- Connects to: First Impression, Customer Journey, and Customer Onboarding Engines.

## Shared Architecture Rules

- Prospect and customer data must have one authoritative record rather than separate engine copies.
- Engines exchange stage changes and approved outputs through defined records.
- Business engines submit approved recommendations to the Decision Engine and receive explainable approved decision packages when a central decision is required.
- Sensitive outbound communication remains subject to human approval.
- Integrations are placeholders until their requirements and access are approved.
- Important architecture decisions belong in `Logs/Decision-Log.md`.
