# Decision Examples

## Purpose

Show how the Decision Engine should explain recommendations. These are hypothetical design examples, not real prospect facts, approved customer content, or authorization to act.

## Example 1: Choose a Personalization Opportunity

**Input:** The Prospect Intelligence Engine provides two human-review-ready opportunities with supporting evidence.

**Decision:** Recommend the opportunity with the stronger verified identity match, recency, professional relevance, and confidence.

**Explanation:** State the evidence used, why the selected opportunity fits the Business Principles, why the alternative ranked lower, and whether human review is required.

**Boundary:** Do not write the First Impression message.

## Example 2: Choose a Featured Property

**Input:** One approved opportunity contains multiple verified properties.

**Decision:** Recommend the approved property most directly connected to the selected opportunity and supported by current evidence.

**Explanation:** Cite the property evidence and selection rules.

**No-action condition:** If ownership of the activity or current status is unclear, recommend no property and require review.

## Example 3: Choose an Approved Image

**Input:** Approved images are available for an approved opportunity.

**Decision:** Recommend the image with verified subject, approved business use, clear opportunity relevance, and appropriate quality.

**Explanation:** Identify the source, approval, relationship to the opportunity, and any limitation.

**No-action condition:** If no image is approved or identity is uncertain, select no image.

## Example 4: Choose the Next Customer Journey Step

**Input:** The authoritative record identifies the current approved journey stage and recorded outcome.

**Decision:** Recommend only the next permitted step in the approved seven-step journey.

**Explanation:** Identify the current stage, completed requirement, and governing journey rule.

**Boundary:** Do not add training, skip steps, or authorize outbound communication.

## Example 5: Choose an Approved Video

**Input:** The current journey step calls for card-creation guidance.

**Decision:** Recommend the approved 3-minute iPhone demonstration as the primary path.

**Alternative:** Recommend the approved 7-minute computer tutorial only when the record shows that the person prefers a computer.

**Explanation:** Cite the approved journey and Business Principle requiring the easiest customer path.

## Example 6: Require Human Review

**Input:** Two eligible actions remain equally supported, or evidence is contradictory.

**Decision:** Require human review.

**Explanation:** List the unresolved conflict, evidence for each option, and the decision that the reviewer must make.

## Example 7: Take No Action

**Input:** Suppression applies, required evidence is missing, no action fits the current journey stage, or action would add unnecessary effort.

**Decision:** No action.

**Explanation:** Cite the controlling suppression, safety, evidence, journey, or Business Principle.

## Example Record Format

Each example decision record should contain:

* Candidate actions
* Selected action or no action
* Supporting evidence
* Rules and Business Principles applied
* Confidence and limitations
* Human-review requirement
* Human override or approval when provided
