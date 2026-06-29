# Human Escalation Flow

## Objective

Transfer the conversation to a human representative when the request cannot be resolved by the AI agent or requires manual intervention.

---

## Flow


---

## Business Rules

- Escalation should occur only after automated recovery attempts fail.
- A service request must be created before transferring the conversation.
- The authenticated session should remain available to the human agent.
- Conversation history should be passed to avoid asking the member to repeat information.
- The agent should clearly inform the user before transferring the call.