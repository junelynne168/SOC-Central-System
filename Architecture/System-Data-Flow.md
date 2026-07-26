# System Data Flow

## Stage Flow

Prospect → Contacted Prospect → Engaged Prospect → Free Card User → Qualified Lead → Customer → Active Relationship Customer

## Stage Definitions

### Prospect

A person who meets approved prospect criteria and has a prospect record.

### Contacted Prospect

A prospect for whom an approved First Impression Email or other approved first contact has been sent.

### Engaged Prospect

A contacted prospect who has shown a recorded engagement signal.

### Free Card User

An engaged prospect who has entered the first-free-card experience or created a free card.

### Qualified Lead

A Free Card User who has demonstrated approved signs of interest in sign-up or personal consultation.

### Customer

A qualified lead whose customer status has been confirmed through the approved sign-up process.

### Active Relationship Customer

A customer participating in approved ongoing relationship marketing.

## Data-Flow Rules

- Maintain one authoritative person record as the individual changes stages.
- Preserve stage history rather than replacing prior outcomes.
- Record the source and time of material stage changes.
- Allow only approved actions for the current stage.
- Require human review for sensitive communication and exceptions.
- Do not interpret provider acceptance as confirmed delivery.
