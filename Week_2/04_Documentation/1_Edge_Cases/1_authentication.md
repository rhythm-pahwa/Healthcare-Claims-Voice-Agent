# Authentication Edge Cases

## Purpose

This document describes the exception scenarios that may occur during member authentication and the expected system behaviour.

---

## Flow

Authentication Agent
        │
        ▼
Collect Member Details
        │
        ▼
Validate Details
        │
        ▼
Authentication Successful?
        │
   ┌────┴─────┐
   │          │
  Yes         No
   │          │
   ▼          ▼
Session     Retry Authentication
Manager          │
           Retry Count < 3 ?
               │
        ┌──────┴──────┐
        │             │
       Yes            No
        │             │
        ▼             ▼
Ask User to      Authentication

Re-enter Details Failure Flow