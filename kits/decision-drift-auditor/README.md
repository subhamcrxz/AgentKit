## Implementation

The Decision Drift Auditor is implemented as a Lamatic.ai workflow.

### Workflow

The workflow consists of three stages:

1. **API Request**
   - Receives a `decisionHistory` input containing organizational decisions and supporting evidence.

2. **Generate Text**
   - Uses an LLM to analyze the decision history.
   - Identifies the original decision, later statements, supporting evidence, potential drift type, confidence, and whether human confirmation is required.
   - The model is instructed not to invent evidence when the history is insufficient.

3. **API Response**
   - Returns a structured audit containing:
     - `decision`
     - `earlierEvidence`
     - `laterEvidence`
     - `driftType`
     - `confidence`
     - `humanConfirmationNeeded`
     - `reason`

### Example

Input:

```json
{
  "decisionHistory": "January 10: Engineering decided PostgreSQL would be the source of truth for customer data. February 15: Architecture confirmed PostgreSQL as the primary customer database. March 3: Engineering and Architecture approved migrating customer-service data to MongoDB, making MongoDB the source of truth for customer-service data."
}
