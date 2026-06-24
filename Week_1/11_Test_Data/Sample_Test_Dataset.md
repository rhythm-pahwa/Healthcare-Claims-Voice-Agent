# Sample Test Dataset

This dataset is created for testing conversational flows during development and validation of the Healthcare Claims Voice Agent.

The data is intended for demonstration and testing purposes only.

## Member Test Data

| Member ID | Name | DOB | ZIP Code | Address | Last 4 SSN |
|------------|------------|------------|------------|------------|------------|
| MEM1001 | John Smith | 15-04-1985 | 10001 | New York | 1234 |
| MEM1002 | Emily Johnson | 22-08-1990 | 60601 | Chicago | 5678 |
| MEM1003 | Michael Brown | 10-12-1982 | 77001 | Houston | 9012 |
| MEM1004 | Sarah Davis | 05-06-1995 | 90001 | Los Angeles | 3456 |
| MEM1005 | David Wilson | 18-09-1988 | 33101 | Miami | 7890 |

## Claim Status Test Data

| Claim ID | Member ID | Claim Type | Claim Status |
|------------|------------|------------|------------|
| CLM1001 | MEM1001 | Medical | Under Review |
| CLM1002 | MEM1002 | Dental | Approved |
| CLM1003 | MEM1003 | Vision | Rejected |
| CLM1004 | MEM1004 | Medical | Processing |
| CLM1005 | MEM1005 | Pharmacy | Approved |

## Eligibility Test Data

| Member ID | Plan Type | Eligibility Status |
|------------|------------|------------|
| MEM1001 | Gold Plan | Eligible |
| MEM1002 | Silver Plan | Eligible |
| MEM1003 | Bronze Plan | Eligible |
| MEM1004 | Gold Plan | Inactive |
| MEM1005 | Silver Plan | Eligible |

## Benefits Test Data

| Member ID | Benefit Type | Coverage |
|------------|------------|------------|
| MEM1001 | Medical | 90% Coverage |
| MEM1002 | Dental | 80% Coverage |
| MEM1003 | Vision | 75% Coverage |
| MEM1004 | Pharmacy | 85% Coverage |
| MEM1005 | Medical | 90% Coverage |

## Provider Lookup Test Data

| Provider ID | Provider Name | Specialty | ZIP Code |
|------------|------------|------------|------------|
| PRV1001 | Dr. James Carter | Cardiology | 10001 |
| PRV1002 | Dr. Sophia Moore | Dermatology | 60601 |
| PRV1003 | Dr. Daniel Clark | Orthopedics | 77001 |
| PRV1004 | Dr. Olivia White | Pediatrics | 90001 |
| PRV1005 | Dr. Ethan Hall | Neurology | 33101 |

## Pre Authorization Test Data

| Authorization ID | Member ID | Procedure | Status |
|------------|------------|------------|------------|
| PA1001 | MEM1001 | MRI Scan | Approved |
| PA1002 | MEM1002 | Surgery | Pending |
| PA1003 | MEM1003 | CT Scan | Approved |
| PA1004 | MEM1004 | Specialist Consultation | Rejected |
| PA1005 | MEM1005 | Physical Therapy | Approved |

## Service Request Test Data

| Ticket ID | Member ID | Issue Type | Status |
|------------|------------|------------|------------|
| SR1001 | MEM1001 | Claim Inquiry | Open |
| SR1002 | MEM1002 | Eligibility Issue | In Progress |
| SR1003 | MEM1003 | Benefits Question | Closed |
| SR1004 | MEM1004 | Provider Lookup Issue | Open |
| SR1005 | MEM1005 | Pre Authorization Query | In Progress |

## Authentication Failure Test Cases

| Scenario ID | Description | Expected Outcome |
|------------|------------|------------|
| AUTH01 | Incorrect DOB | Retry Authentication |
| AUTH02 | Incorrect ZIP Code | Retry Authentication |
| AUTH03 | Incorrect SSN | Retry Authentication |
| AUTH04 | Three Failed Attempts | Human Escalation |
| AUTH05 | Missing Authentication Data | Authentication Failure |

## Intent Recognition Test Cases

| Test Case ID | User Request | Expected Intent |
|------------|------------|------------|
| INT01 | I want to check my claim status | Claim Status |
| INT02 | Submit a new claim | Claim Submission |
| INT03 | Check my eligibility | Eligibility Check |
| INT04 | Tell me my benefits | Benefits Inquiry |
| INT05 | Find a provider near me | Provider Lookup |
| INT06 | Check my pre authorization status | Pre Authorization Status |
| INT07 | I need help from an agent | Human Escalation |
