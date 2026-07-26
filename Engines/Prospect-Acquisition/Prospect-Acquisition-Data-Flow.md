# Prospect Acquisition Data Flow

## Primary Flow

Public Source  
→ Candidate Record  
→ Evidence Collection  
→ Duplicate Check  
→ Validation  
→ Scoring  
→ Human Review  
→ Approved Prospect Record  
→ First Impression Engine

## Stage Responsibilities

1. **Public Source:** An approved public source presents candidate business information.
2. **Candidate Record:** Create a provisional record linked to its source evidence.
3. **Evidence Collection:** Collect only approved public business facts, source references, and review timestamps.
4. **Duplicate Check:** Compare the candidate with authoritative prospect and customer records.
5. **Validation:** Confirm required fields, business-use context, source reliability, and suppression status.
6. **Scoring:** Apply the approved framework using documented evidence.
7. **Human Review:** Review the complete candidate, evidence, score, duplicate result, suppression status, and personalization opportunity.
8. **Approved Prospect Record:** Record the approved outcome in the authoritative prospect record.
9. **First Impression Engine:** Transfer only the approved prospect record and its required evidence. Movement to this engine does not by itself authorize sending.

## Exception Paths

| Exception | Required path |
|---|---|
| Missing contact information | Stop advancement; mark incomplete and record what is missing |
| Contradictory data | Stop advancement; preserve each source and route to human review |
| Duplicate records | Stop new-record advancement; record the match result and require human review without automatic merging |
| Suppression status | Stop contact progression; preserve the suppression evidence and route according to approved policy |
| Unverified recent activity | Do not award unsupported activity points; mark incomplete, deferred, or route for human review |
| Source unavailable | Record the failure and timestamp; use another approved source only when permitted, otherwise mark incomplete or deferred |

## Data Rules

* Use one authoritative prospect record.
* Preserve source evidence and stage history.
* Never invent missing facts.
* Never bypass duplicate, validation, suppression, or human-review gates.
* Do not send communication from this engine.
