Analyze the following decision history for decision drift.
Decision history:
{{triggerNode_1.output.decisionHistory}}
Identify:
1. The original decision.
2. Later statements or decisions that change or contradict it.
3. Evidence supporting each potential conflict.
4. Whether the change appears intentional, uncertain, or contradictory.
5. Which decisions require human confirmation.
Do not invent facts. If evidence is insufficient, say so clearly.
Return ONLY valid JSON in this exact structure:
{
"decision": "The original decision",
"earlierEvidence": "Evidence supporting the original decision",
"laterEvidence": "Evidence showing the later decision or statement",
"driftType": "None | Change | Contradiction | Uncertain",
"confidence": "High | Medium | Low",
"humanConfirmationNeeded": true,
"reason": "Brief explanation"
}