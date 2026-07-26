# Prospect-to-Customer Workflow

## Purpose

Provide the single master business workflow for the SOC Central System.

This document is the primary business workflow used by Atlas, Codex, June, and future SOC partners. It connects every approved engine into one continuous process while preserving the approved customer journey.

## Complete Workflow

Prospect Found  
↓  
Prospect Acquisition Engine  
↓  
Prospect Intelligence Engine  
↓  
Decision Engine  
↓  
First Impression Email (validated internal test)  
↓  
Email Delivered  
↓  
Decision Point: Did the prospect open the email?

**If NO**  
↓  
Follow-up Strategy (future engine placeholder)

**If YES**  
↓  
30-second SOC Introduction  
↓  
Create Your First FREE Card  
↓  
3-minute iPhone Demonstration  
↓  
Send First Card  
↓  
Experience Result  
↓  
Optional 7-minute Computer Tutorial  
↓  
Appointment / Online Sign-up  
↓  
Customer  
↓  
Customer Onboarding Engine  
↓  
Relationship Generator Engine  
↓  
Long-term Relationship Marketing

The Customer Journey Engine coordinates the approved journey stages and records outcomes. The AI Video Production System supplies the approved 30-second introduction, primary 3-minute iPhone demonstration, and optional 7-minute computer tutorial. The Decision Engine makes supported central decisions; it does not replace the primary responsibility of another engine.

## Decision Points

### Email opened?

* **Positive path:** Record the engagement and present the approved 30-second SOC Introduction.
* **Negative path:** Take no unapproved action; retain the Contacted Prospect state and route the record for an approved follow-up decision.
* **Future automation placeholder:** Follow-up Strategy after First Impression. Requirements are not designed here.

### CTA clicked?

* **Positive path:** Guide the engaged prospect into **Create Your First FREE Card**.
* **Negative path:** Preserve the Engaged Prospect state and wait for an approved follow-up decision.
* **Future automation placeholder:** CTA follow-up timing and reminder rules. Requirements are not designed here.

### Free card created?

* **Positive path:** Guide the Free Card User with the primary 3-minute iPhone demonstration toward sending the first card.
* **Negative path:** Preserve progress and route the record for approved assistance or follow-up.
* **Future automation placeholder:** Incomplete free-card assistance and reminder rules. Requirements are not designed here.

### First card sent?

* **Positive path:** Record the experience result and continue toward the optional computer tutorial, appointment, or online sign-up as appropriate.
* **Negative path:** Keep the person in the Free Card User state and route the record for approved assistance.
* **Future automation placeholder:** First-card completion assistance and follow-up rules. Requirements are not designed here.

### Appointment booked?

* **Positive path:** Record the appointment and treat the person as a Qualified Lead pending the approved consultation outcome.
* **Negative path:** Keep online sign-up available and take no additional action without an approved next-step decision.
* **Future automation placeholder:** Appointment invitation, scheduling, and follow-up rules. Requirements are not designed here.

### Customer signed up?

* **Positive path:** Record the Customer state and begin the approved Customer Onboarding Engine workflow.
* **Negative path:** Preserve the Qualified Lead state when its entry conditions remain met; otherwise preserve the current verified state.
* **Future automation placeholder:** Sign-up follow-up and qualified-lead nurture rules. Requirements are not designed here.

## Engine Responsibilities

| Engine | Input | Output | Next Engine |
| --- | --- | --- | --- |
| Prospect Acquisition Engine | Prospect found, approved criteria, permitted public sources, existing records, and suppression status | Human-approved prospect record with source, score, duplicate, suppression, and review evidence | Prospect Intelligence Engine |
| Prospect Intelligence Engine | Approved prospect record and verified supporting evidence | Human-approved personalization recommendation, confidence, and evidence | Decision Engine |
| Decision Engine | Approved recommendation, authoritative record, journey stage, evidence, and safety status | Explainable best next action or no action, including human-review requirement | Appropriate business engine; initially First Impression Engine |
| First Impression Engine | Approved prospect record, approved decision, intelligence package, messaging, and assets | Human-approved First Impression Email, send and delivery evidence, and engagement signals | Customer Journey Engine and Decision Engine |
| Customer Journey Engine | Current state, engagement, recorded outcomes, and approved journey rules | Stage history, next approved journey action, and exceptions | Decision Engine and the engine responsible for the next step |
| Customer Onboarding Engine | Engaged prospect record, free-card access, approved demonstrations, and recorded outcomes | Free-card, first-card, appointment, sign-up, and onboarding outcomes | Decision Engine or Relationship Generator Engine |
| Relationship Generator Engine | Authoritative customer record, approved relationship context, milestones, and review rules | Human-reviewed relationship opportunities and recorded outcomes | Decision Engine and Customer Journey Engine |
| AI Video Production System | Approved scripts, demonstration requirements, brand requirements, and review decisions | Approved 30-second introduction, 3-minute iPhone demonstration, optional 7-minute computer tutorial, and future approved videos | Decision Engine and the business engine presenting the approved video |

## Customer State Table

| Customer state | Entry condition | Exit condition | Responsible engine |
| --- | --- | --- | --- |
| Prospect | Person meets approved prospect criteria and has an authoritative prospect record | Approved First Impression contact is sent and recorded | Prospect Acquisition Engine |
| Contacted Prospect | Approved First Impression Email or other approved first contact is sent | A recorded engagement signal is confirmed | First Impression Engine |
| Engaged Prospect | Contacted prospect opens, clicks, responds, or shows another approved engagement signal | Person enters or creates the first-free-card experience | Customer Journey Engine |
| Free Card User | Engaged prospect enters the first-free-card experience or creates a free card | Approved qualification evidence is recorded after card creation, card sending, appointment interest, or sign-up interest | Customer Onboarding Engine |
| Qualified Lead | Free Card User demonstrates approved interest in sign-up or personal consultation | Customer sign-up is confirmed, or qualification is withdrawn through an approved review | Customer Onboarding Engine |
| Customer | Qualified Lead completes the approved sign-up process | Approved ongoing relationship-marketing participation begins | Customer Onboarding Engine |
| Active Relationship Customer | Customer participates in approved ongoing relationship marketing | Relationship status changes through an approved recorded decision | Relationship Generator Engine |

The Decision Engine supports transitions but does not own the authoritative person record or replace the responsible engine.

## Workflow Rules

* Never skip approved customer journey steps.
* Give the person one clear next action.
* Require human review where approved rules require it.
* Preserve one authoritative prospect and customer record.
* Every engine performs one primary responsibility.
* Decisions belong to the Decision Engine.
* Customer-facing content belongs only to the appropriate engine.
* Never treat provider acceptance as confirmed email delivery.
* The future Follow-up Strategy remains a placeholder until separately approved.

## Visual Workflow

```text
Prospect Found
      |
      v
[Prospect Acquisition]
      |
      v
[Prospect Intelligence]
      |
      v
[Decision Engine]
      |
      v
[First Impression Email] ---> Delivered? ---> [Customer Journey records state]
      |                                             |
      v                                             v
 Email opened? -- NO --> [Future Follow-up Strategy placeholder]
      |
     YES
      |
      v
[30-second SOC Introduction] <--- [AI Video Production]
      |
      v
[Create Your First FREE Card] ---> CTA clicked? -- NO --> [Future approved follow-up]
      |
     YES
      |
      v
 Free card created? -- NO --> [Future approved assistance]
      |
     YES
      |
      v
[3-minute iPhone Demonstration] <--- [AI Video Production]
      |
      v
[Send First Card] ---> First card sent? -- NO --> [Future approved assistance]
      |
     YES
      |
      v
[Experience Result]
      |
      +--> [Optional 7-minute Computer Tutorial] <--- [AI Video Production]
      |
      v
[Appointment / Online Sign-up]
      |
      +--> Appointment booked? -- NO --> [Online sign-up remains available]
      |
      v
 Customer signed up? -- NO --> [Qualified Lead or current verified state]
      |
     YES
      |
      v
   [Customer]
      |
      v
[Customer Onboarding]
      |
      v
[Relationship Generator]
      |
      v
Long-term Relationship Marketing

Decision Engine: selects supported next actions or no action at decision points.
Customer Journey Engine: coordinates approved stages and preserves state history.
```

## Design Status

This is a design-only master workflow. It does not authorize automation, communication, a new engine, or changes to the approved customer journey.
