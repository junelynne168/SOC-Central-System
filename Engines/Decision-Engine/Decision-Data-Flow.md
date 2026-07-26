# Decision Data Flow

## Central Flow

Approved Business-Engine Recommendation  
→ Authoritative Record Check  
→ Suppression and Safety Gate  
→ Evidence and Eligibility Validation  
→ Business-Principles Review  
→ Decision Rules  
→ Best Next Action or No Action  
→ Explanation and Review Requirement  
→ Human Review When Required  
→ Approved Decision Package  
→ Appropriate Business Engine

## Connected Business Engines

The Decision Engine receives approved recommendations from and returns approved decision packages to:

* Prospect Acquisition Engine
* Prospect Intelligence Engine
* First Impression Engine
* Customer Journey Engine
* Customer Onboarding Engine
* Relationship Generator Engine
* AI Video Production System

## Input Package

* Source engine
* Authoritative prospect or customer identifier
* Current journey stage
* Approved recommendation or candidate actions
* Supporting evidence
* Confidence and limitations
* Suppression and safety status
* Human-review status
* Approved assets or references required by the action

## Output Package

* Selected action or no action
* Destination engine
* Supporting evidence
* Applied rules and Business Principles
* Explanation and confidence
* Human-review requirement and outcome
* Decision timestamp and status

## Exception Paths

| Exception | Required path |
|---|---|
| Suppression or safety block | Stop and return no action with the controlling rule |
| Missing evidence | Mark incomplete and request approved evidence |
| Contradictory evidence | Preserve conflicts and require human review |
| Invalid journey action | Reject the action and identify the permitted current step |
| Missing approved asset | Do not select the asset; return incomplete or choose no action |
| Multiple equally suitable actions | Require human review |
| No eligible action | Record no action and explain why |
| Rule conflict | Stop and require human review; do not guess |

## Data Rules

* Do not duplicate the authoritative person record.
* Preserve source-engine recommendations and decision history.
* Separate verified facts, approved recommendations, AI rankings, and human decisions.
* Never create customer-facing content or send communication.
