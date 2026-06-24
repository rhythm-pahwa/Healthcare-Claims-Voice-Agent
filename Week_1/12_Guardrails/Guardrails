# Agent Guidelines & Guardrails

| Guardrail Area | Description | Agent Action |
|---------------|-------------|-------------|
| Input Validation | Accept only supported healthcare-related requests. Block malicious, abusive, irrelevant, or unauthorized requests. | Reject invalid input and offer escalation if needed. |
| Authentication | Verify member identity before accessing protected information. | Collect Member ID, DOB, ZIP Code, and Last 4 Digits of SSN. |
| Authentication Failure | Prevent unauthorized access to member data. | Allow maximum 3 attempts, then escalate to human agent. |
| Session Management | Maintain secure user sessions. | Require re-authentication after timeout or inactive session. |
| Intent Classification | Identify the user's purpose accurately. | Classify intent and route to the appropriate domain. |
| Confidence Scoring | Ensure correct routing decisions. | High Confidence (>85%) → Route. Medium (70-85%) → Clarify. Low (<70%) → Escalate. |
| Domain Routing | Route requests only to approved healthcare domains. | Claims, Eligibility, Benefits, Provider Lookup, Pre-Authorization, Escalation. |
| API / Tool Execution | Prevent incorrect or fabricated information. | Use approved APIs only and validate responses before presenting results. |
| Authorization Validation | Ensure requested data belongs to authenticated member. | Verify claim ownership before disclosure. |
| PHI Protection | Protect sensitive healthcare information. | Never disclose PHI before successful authentication. |
| Data Masking | Prevent exposure of sensitive identifiers. | Mask Member IDs, Claim IDs, SSN, and Phone Numbers. |
| Response Delivery | Provide accurate and minimal necessary information. | Share only relevant information returned from verified systems. |
| No Input / Silence | Handle inactive callers. | Reprompt user and terminate or escalate after repeated silence. |
| Unclear Speech | Handle low-quality voice input. | Ask the caller to repeat or clarify. |
| User Interruptions | Support natural conversation flow. | Pause current response and process interruption. |
| Change of Intent | Support multi-purpose conversations. | Reclassify intent and route to correct workflow. |
| User Cancellation | Respect cancellation requests. | Stop current workflow and confirm cancellation. |
| Long Conversations | Prevent context overflow. | Summarize context and continue or escalate. |
| Backend API Error | Handle system failures gracefully. | Retry operation and escalate if unresolved. |
| System Timeout | Handle delayed responses from systems. | Inform user and retry where applicable. |
| Service Unavailable | Handle unavailable backend services. | Create service request and escalate. |
| Human Escalation | Ensure unresolved issues are handled safely. | Transfer to human representative with conversation summary. |
| Conversation Closure | End interactions professionally. | Confirm completion and close conversation politely. |

---

## Escalation Triggers

| Trigger | Action |
|----------|----------|
| Authentication Failed 3 Times | Human Agent Escalation |
| Confidence Score Below 70% | Human Agent Escalation |
| User Requests Human Agent | Immediate Escalation |
| Claim Ownership Cannot Be Verified | Escalation |
| Backend API Failure | Escalation |
| Service Unavailable | Escalation |
| Sensitive Disputes or Complaints | Escalation |
| Unexpected System Error | Escalation |

---

## Confidence Score Rules

| Confidence Level | Range | Action |
|-----------------|--------|---------|
| High | > 85% | Route directly to domain supervisor |
| Medium | 70% - 85% | Ask clarification questions and re-evaluate |
| Low | < 70% | Escalate to human agent |

---

## Supported Domains

| Domain Supervisor | Responsibilities |
|------------------|------------------|
| Claims Sub-Supervisor | Claim Status, Claim History, Claim Tracking |
| Eligibility Sub-Supervisor | Coverage Verification, Eligibility Checks |
| Benefits Sub-Supervisor | Benefits Information, Coverage Details |
| Provider Lookup Sub-Supervisor | Provider Search, Network Verification |
| Pre-Authorization Sub-Supervisor | Authorization Status, Authorization Requirements |
| Escalation Sub-Supervisor | Human Agent Requests, Complex Cases |