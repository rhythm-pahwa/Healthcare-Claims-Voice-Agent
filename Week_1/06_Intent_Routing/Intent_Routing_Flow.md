# Intent Routing Flow

The Intent Routing Flow is responsible for identifying the user's request and directing the conversation to the appropriate healthcare service journey.

After the user provides their request, the voice agent analyzes the conversation and determines the most relevant intent. Once the intent is identified, the conversation is routed to the corresponding service flow.

If the intent cannot be identified, the voice agent attempts to clarify the user's request. If the request remains unclear after multiple attempts, the conversation is escalated to a human representative.

## Supported Intents

The following intents were identified during requirement analysis:

- Claim Status
- Claim Submission
- Eligibility Check
- Benefits Inquiry
- Provider Lookup
- Pre Authorization Status
- Service Request
- Agent Escalation

## Intent Identification Process

The voice agent performs the following steps:

1. Capture the user's request.
2. Analyze the request.
3. Identify the most relevant intent.
4. Determine whether authentication is required.
5. Route the conversation to the appropriate service flow.

## Unknown Intent Handling

If the user's request is unclear:

1. Ask the user to rephrase the request.
2. Attempt intent identification again.
3. Present supported services if necessary.
4. Escalate to a human representative if the intent cannot be determined.

## Routing Logic

Claim Status
→ Authentication Flow
→ Claim Status Journey

Claim Submission
→ Authentication Flow
→ Claim Submission Journey

Eligibility Check
→ Authentication Flow
→ Eligibility Journey

Benefits Inquiry
→ Authentication Flow
→ Benefits Journey

Provider Lookup
→ Authentication Flow
→ Provider Lookup Journey

Pre Authorization Status
→ Authentication Flow
→ Pre Authorization Journey

Service Request
→ Authentication Flow
→ Service Request Journey

Agent Escalation
→ Human Agent Escalation Flow

## Flow Diagram

![Intent Routing Flow](../All_FLows/Intent_routing_flow.png)

## Flow Summary

- Identify user intent.
- Handle unsupported requests.
- Route users to the correct healthcare journey.
- Trigger authentication when required.
- Escalate unclear requests when necessary.
