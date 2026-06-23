# Claim Status Journey

The Claim Status Journey allows authenticated users to retrieve the current status of a submitted healthcare claim.

The user must complete authentication and identity verification before claim information is disclosed.

## Happy Path Conversation

User:
I would like to check my claim status.

Bot:
I can help you with that. Please complete identity verification.

Authentication Completed

Bot:
Please provide your Claim ID.

User:
CLM10234

Bot:
Retrieving your claim information.

Bot:
Your claim has been received and is currently under review.

Bot:
Is there anything else I can help you with today?

## Flow Summary

- User requests claim status.
- User completes authentication.
- Claim ID is collected.
- Claim information is retrieved.
- Claim status is provided.
- Additional assistance is offered.

## Flow Diagram

![Claim Status Flow](../assets/Claim_Status.png)
