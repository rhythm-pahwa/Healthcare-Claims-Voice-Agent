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