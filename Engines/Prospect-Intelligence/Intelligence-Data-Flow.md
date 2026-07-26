# Intelligence Data Flow

## Primary Flow

Approved Prospect Record  
→ Approval and Safety Check  
→ Verified Fact Set  
→ Opportunity Analysis  
→ Personalization Scoring  
→ Recommendation Package  
→ Human Review  
→ Approved Intelligence Package  
→ First Impression Engine

## Data Responsibilities

1. **Approved Prospect Record:** Receive the authoritative approved record and its evidence without creating a duplicate customer record.
2. **Approval and Safety Check:** Confirm prospect approval, duplicate result, and suppression status before analysis.
3. **Verified Fact Set:** Separate evidence-backed approved facts from AI suggestions and unusable information.
4. **Opportunity Analysis:** Identify possible professional personalization opportunities.
5. **Personalization Scoring:** Score evidence quality and opportunity usefulness, then assign an explained confidence level.
6. **Recommendation Package:** Assemble suggested opportunity outputs with facts, evidence, labels, limitations, and score.
7. **Human Review:** Approve, reject, defer, or mark the recommendation incomplete.
8. **Approved Intelligence Package:** Record the selected recommendation and review decision with the authoritative prospect record.
9. **First Impression Engine:** Receive only the human-approved intelligence package needed to prepare customer-facing content.

## Exception Paths

| Exception | Required path |
|---|---|
| Prospect not approved | Stop; return to the Prospect Acquisition review state |
| Suppression or safety conflict | Stop; preserve status and route for human review |
| Missing supporting evidence | Mark the recommendation incomplete; do not infer facts |
| Contradictory facts | Preserve each source, exclude the disputed fact, and route for human review |
| No meaningful opportunity | Record that no recommendation is available; do not force personalization |
| Low confidence | Do not advance without additional approved evidence and human review |
| Source reference unavailable | Record the unavailable source and use no unsupported fact |

## Handoff Package

The First Impression Engine may receive:

* Prospect identifier
* Human-approved recommendation
* Verified supporting facts
* Evidence references
* Suggested featured property, congratulation opportunity, and photo when approved
* Suggested opening theme and relationship angle
* Confidence level and explanation
* Human-review decision and timestamp

The handoff contains no generated customer message and does not authorize outbound communication.
