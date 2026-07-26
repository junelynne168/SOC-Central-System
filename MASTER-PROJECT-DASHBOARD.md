# SOC Central System Dashboard

This is the authoritative project overview and the first document Atlas, Codex, and June review before continuing SOC Central System work.

## 1. Project Status

**Current Phase:**

**Business Operations Design**

**Previous Phase:**

**Architecture Design (Completed)**

**Overall Progress:**

60% estimated

**Last Updated:**

2026-07-26

**Current Project Health:**

**BLOCKED — GitHub CLI is installed and the repository choices are approved, but GitHub rejects the saved `junelynne168` token as invalid. June must reauthorize GitHub CLI before deployment can proceed.**

---

## 2. Engine Status

| Engine | Status | Atlas Review | Codex Status | Comment |
| ------ | ------ | ------------ | ------------ | ------- |
| Prospect Acquisition | Approved | Approved | Completed | V1 design approved. |
| Prospect Intelligence | Approved | Approved | Completed | Personalization-layer design approved. |
| Decision Engine | Approved | Approved | Completed | Central decision-layer design approved. |
| First Impression | Approved | Approved | Completed | Email #1 validated. Email #2 V1.3 is Production Approved; Internal Test #3 passed. |
| First FREE Card Experience | Waiting Review | Approved | Blocked | Production-ready landing page implemented locally. Public test deployment is blocked pending a connected GitHub repository and authenticated GitHub Pages access. |
| Customer Journey | Approved | Approved | Completed | Approved seven-step journey preserved. |
| Prospect-to-Customer Workflow | Approved | Approved | Completed | Master business workflow approved. |
| Customer Onboarding | Planned | Planned | Planned | Business operations design remains. |
| Relationship Generator | Planned | Planned | Planned | Business operations design remains. |
| AI Video Production | Planned | Planned | Planned | Operational video requirements remain. |

Allowed status values:

* Planned
* Designing
* Waiting Review
* Approved
* Implementing
* Testing
* Validated
* Completed

**Validated:** Successfully proven through real or internal testing.

---

## 3. Architecture Documents

| Document | Status |
| --- | --- |
| `Architecture/Business-Principles.md` | Approved |
| `Architecture/Customer-Journey.md` | Approved |
| `Architecture/Experience-Driven-Design.md` | Approved |
| `Architecture/Integration-Map.md` | Approved |
| `Architecture/Prospect-to-Customer-Workflow.md` | Approved |
| `Architecture/SOC-Partner-Ready-Design.md` | Approved |
| `Architecture/System-Architecture.md` | Approved |
| `Architecture/System-Data-Flow.md` | Approved |

---

## Production Artifacts

Reference: `Production/Production-Catalog.md`

---

## 4. Major Decisions

* **AI is not the product:** A simpler business is the product.
* **Create Your First FREE Card:** Let prospects experience value before asking them to buy.
* **Mobile First:** The 3-minute iPhone demonstration is primary; the computer tutorial is optional.
* **SOC First:** Complete the simplest reliable SOC system before considering other industries.
* **Partner Ready:** Keep shared SOC logic stable and place partner information in configuration.
* **Decision Engine:** Use one explainable, evidence-backed, human-overridable decision layer.
* **Prospect Intelligence:** Personalization recommendations sit between Prospect Acquisition and First Impression.
* **Experience-Driven Design:** The SOC system is designed around customer experiences before software implementation.

See `Logs/Decision-Log.md` for the authoritative decision history.

---

## 5. Existing Validated Work

* First Impression Email internally tested successfully.
* Internal email delivery validated.
* Internal Test #2 = Sent
  * Gmail timestamp: `2026-07-26T15:57:12`
  * Gmail Message ID: `19f9f250b5c66eb2`
  * Recipient: `June.Lynne168@gmail.com`
  * Subject: `Bobbi, a quick thought`
  * Exact HTML: `Engines/First-Impression/Approved-First-Impression-Email.html`
  * Reply Received = Yes
  * Reply Gmail Message ID: `19f9f281ed05a1d3`
  * Reply timestamp: `2026-07-26T16:00:22`
  * Thread ID: `19f9f250b5c66eb2`
* Internal Test #3 = Blocked before send
  * Attempted recipient: `June.Lynne168@gmail.com`
  * Approved subject: `Here's the 30-second idea I promised`
  * Existing Thread ID: `19f9f250b5c66eb2`
  * Gmail result: `Failed to build message payload — Subject does not match`
  * Gmail Message ID: Not created
  * Send timestamp: Not created
* Internal Test #3 = Sent as a new thread
  * Gmail timestamp: `2026-07-26T16:43:37`
  * Gmail Message ID: `19f9f4f87dd1ccba`
  * Thread ID: `19f9f4f87dd1ccba`
  * Recipient: `June.Lynne168@gmail.com`
  * Subject: `Here's the 30-second idea I promised`
  * Exact HTML: `Engines/Second-Impression/Email-2.html`
  * SHA-256 before send: `D5C098E1EF7E580CCD0C44B01023DE669C464A9F86D999B0988BD5A071DEA2F7`
  * Status: **RECEIVED — LINK TEST FAILED**
  * Visual appearance: Good, confirmed by June
  * Link result: All three links failed because placeholder URLs remain
  * Missing assets report: `Engines/Second-Impression/MISSING-LINK-ASSETS-REPORT.md`
  * Production link library: `Assets/Production-Links.md`
  * Email #2 status: **Waiting for 30-second video URL**
* Internal Test #3 Retest = Sent
  * Gmail timestamp: `2026-07-26T18:20:48`
  * Gmail Message ID: `19f9fa8814c23436`
  * Thread ID: `19f9fa8814c23436`
  * Recipient: `June.Lynne168@gmail.com`
  * Subject: `Here's the 30-second idea I promised`
  * Exact HTML: `Engines/Second-Impression/Email-2.html`
  * SHA-256 before send: `8377F01358E35B293C24B97C4528CB00B03B079D66B65693BAD82AFF6BA5F796`
  * Link validation: All four approved HTTPS URLs present; zero unresolved placeholders in Email #2 sources
  * Status: **Waiting for June's link verification**
* Email #2 V1.2 Final Text Refinement = Implemented
  * Added: `Need help? Watch this quick 5-minute video.`
  * Placement: Immediately below `Create My First FREE Card` and immediately above the existing 5-minute iPhone tutorial link
  * Subject, other wording, URLs, layout, and branding preserved
  * Send status: **Not sent**
  * Review status: **Waiting for June's review**
* Email #2 V1.3 Final Retest = Passed
  * Gmail timestamp: `2026-07-26T18:36:54`
  * Gmail Message ID: `19f9fb73f5bf9cab`
  * Thread ID: `19f9fb73f5bf9cab`
  * Recipient: `June.Lynne168@gmail.com`
  * Subject: `Here's the 30-second idea I promised`
  * Exact HTML: `Engines/Second-Impression/Email-2.html`
  * SHA-256 before send: `60F864C29E2911593770F29BF508E0F99FAD18A4198D2CB935D709EADB4A7C54`
  * Pre-send validation: Approved V1.3 sequence confirmed; all four HTTPS links present; zero unresolved placeholders
  * Email received successfully: **Yes**
  * All four production links verified by June: **Yes**
  * Visual layout approved: **Yes**
  * Customer journey approved: **Yes**
  * Internal Test #3: **Passed**
  * Email #2 status: **Production Approved**
  * Production baseline Markdown: `Engines/Second-Impression/Email-2.md`
  * Markdown SHA-256: `CE9B2B0B2A98EC45D4E70E781EAB1AA8B434F2AF549ECA3979B439D1F4F32A48`
  * Production baseline HTML: `Engines/Second-Impression/Email-2.html`
  * HTML SHA-256: `60F864C29E2911593770F29BF508E0F99FAD18A4198D2CB935D709EADB4A7C54`
  * Freeze rule: Do not modify either baseline production artifact unless June explicitly approves a future revision.
* First FREE Card Landing Page deployment = Blocked
  * Approved local source: `Engines/First-FREE-Card-Experience/Production/Landing-Page/`
  * Requested deployment method: GitHub Pages
  * Hosted landing-page URL: Not created
  * Blocker: GitHub CLI reports the active `junelynne168` token is invalid; repository access returns HTTP 401
  * Approved repository: `junelynne168/SOC-Central-System` (Private)
  * Approved scope: Only `C:\AI-Headquarters-Workspace\Projects\Business\SOC-Central-System`
  * Repository scope risk: The existing Git root is the entire `C:\AI-Headquarters-Workspace`; it contains unrelated and uncommitted work and must not be published as the SOC repository without explicit approval
  * Local path validation: `styles.css`, `script.js`, and `assets/hero-kitchen-temporary.png` use valid relative paths and exist
  * Landing-page CTA validation: Both buttons point to `https://www.SendOutCards.com/u/StayInTouch`
  * Email #2 V1.4: Not created
  * Gmail Message ID: Not created
  * Gmail Thread ID: Not created
  * Send timestamp: Not created
  * Blocker report: `Engines/First-FREE-Card-Experience/Production/Landing-Page/LANDING-PAGE-DEPLOYMENT-BLOCKER.md`
* Approved First Impression Email artifact recovered.
  * `Engines/First-Impression/Approved-First-Impression-Email.md`
  * `Engines/First-Impression/Approved-First-Impression-Email.html`
* Customer Journey approved.
* Architecture approved.
* Prospect-to-Customer Workflow approved.

These items must be preserved and must not be redesigned without June’s explicit approval.

---

## 6. Current Focus

First FREE Card Landing Page Deployment Blocker

---

## 7. Next Recommended Task

June reauthorizes GitHub CLI with `& "C:\Program Files\GitHub CLI\gh.exe" auth login -h github.com -p https -w`, verifies `gh auth status`, and tells Codex it succeeded.

Atlas should update this single task whenever a design milestone is completed.

---

## 8. Parking Lot

Ideas intentionally postponed:

* Multi-industry platform
* Insurance version
* Mortgage version
* Financial Advisor version

Remember these ideas, but do not allow them to affect the current SOC architecture.

---

**Atlas Rule #0: Keep responses short. Action first.**

# Atlas Rule #1

Before proposing, designing, modifying, reviewing, or implementing any SOC work, Atlas must first review this dashboard.

Atlas must report:

1. Current Phase
2. Current Focus
3. Last Completed Milestone
4. Next Recommended Task
5. Current Project Health (blockers, inconsistencies, or pending approvals)

Only after this review may Atlas recommend the next action.

The dashboard is the single source of truth.

Memory must never override the dashboard.

# Atlas Rule #2

A project milestone is **not complete** until all required project documentation has been updated.

After every approved design, implementation, validation, or status change, Atlas must ensure:

1. MASTER-PROJECT-DASHBOARD.md is updated.
2. Logs/Decision-Log.md is updated when appropriate.
3. Related project documents are updated when affected.
4. Status values remain consistent across all project documents.
5. Current Focus and Next Recommended Task are reviewed.
6. Existing Validated Work is updated when applicable.

The Dashboard must always reflect the true current state of the project.

---

# Atlas Rule #7

Before proposing, designing, or implementing any feature:

1. Check `Production/Production-Catalog.md`.
2. If a Production Approved version exists:
   - Reuse it.
   - Do not redesign it.
3. A production artifact may only change after June explicitly approves a new version.

---

# Atlas Rule #8

Before Atlas proposes any new page, feature, automation, or workflow:

1. Identify the customer experience.
2. Define:
   - Emotion
   - Question
   - Action
3. Obtain June's approval.
4. Only then proceed with implementation.

---

## 9. Atlas Working Rules

Before suggesting new work, Atlas must check:

1. Has this already been designed?
2. Has Codex already created it?
3. Has Atlas already approved it?
4. Is it listed as completed or validated?
5. Is there a simpler way?

If yes, do not redesign.

## Update Rules

Whenever a milestone is approved, update:

* Project Progress
* Engine Status
* Current Focus
* Next Recommended Task
* Existing Validated Work, if applicable
* Validated artifact audit before every release

Do not update historical approvals manually outside the dashboard.
