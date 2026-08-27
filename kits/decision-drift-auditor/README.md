# Decision Drift Auditor

## Overview

Decision Drift Auditor analyzes an organization's decision history to identify changes in direction, contradictions, inconsistencies, and recurring decision-making patterns.

## Input

The agent accepts:

- `decisionHistory` — a string containing the organization's decision history.

## What It Does

The auditor:

1. Reviews the provided decision history.
2. Identifies significant changes in decisions or direction.
3. Detects conflicts and contradictions.
4. Finds recurring patterns and inconsistencies.
5. Explains the evidence behind each finding.
6. Provides practical recommendations.

## Output

The audit contains:

- **Summary**
- **Detected Decision Drift**
- **Conflicts or Contradictions**
- **Evidence**
- **Recommendations**

The auditor must rely only on information contained in the supplied decision history and must not invent unsupported facts.
