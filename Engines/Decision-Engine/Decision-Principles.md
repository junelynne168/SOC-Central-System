# Decision Principles

## Purpose

Define the permanent principles for recommendations made by the central Decision Engine.

## Governing Principles

### 1. Never Invent Facts

Use only approved facts and approved recommendations supported by recorded evidence. Missing information must remain missing.

### 2. Safety and Suppression Come First

Never override suppression, do-not-contact, consent, destination, security, or other approved safety controls. When a safety requirement is unresolved, recommend no action or human review.

### 3. Follow the Business Principles

Every decision must follow `../../Architecture/Business-Principles.md`, including simplicity, low customer effort, one clear next action, valuable human attention, and the approved connected journey.

### 4. Require Supporting Evidence

Every decision must cite the facts, approved recommendations, and rules that support it. Unsupported options are ineligible.

### 5. Make Decisions Explainable

Record what was selected, which alternatives were considered, why they were accepted or rejected, which rules applied, and what uncertainty remains.

### 6. Human Approval Overrides AI Recommendations

A human reviewer may approve, reject, replace, defer, or stop a recommendation. Record the reviewer’s decision and reason.

### 7. No Action Is a Valid Decision

Recommend no action when evidence, approval, safety, timing, or journey fit is insufficient.

### 8. Preserve the Approved Journey

Select only steps and actions permitted by the current approved customer journey. Do not insert, remove, reorder, or redesign journey steps.

### 9. Use One Authoritative Record

Read and record decisions against the authoritative prospect or customer record rather than creating duplicate person records.

### 10. Keep the Decision Simple

Choose one clear next action when one is justified. Do not create unnecessary branches, content, or complexity.

## Design Status

These principles govern the design. Decision automation requires separate approval.
