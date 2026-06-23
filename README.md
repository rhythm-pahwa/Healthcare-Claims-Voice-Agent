# Healthcare Claims Voice Agent

## Team Members

- Rhythm
- Neha
- Ramaz
- Pragati
- Palak

## Overview

Healthcare contact centers receive a high volume of member and provider calls related to claim status, claim submission, eligibility verification, benefits inquiries, provider lookup, pre authorization requests, and service requests.

This project focuses on designing a HIPAA compliant Healthcare Claims Voice Agent using CX Agent Studio and multi agent orchestration. The solution aims to provide secure authentication, accurate intent identification, conversational routing, and human agent escalation when required.

## Objectives

- Design secure conversational flows
- Support healthcare claims related services
- Enable user authentication and verification
- Protect sensitive healthcare information
- Improve member and provider experience
- Support escalation to human agents when necessary

## Core Intents

- Claim Status
- Claim Submission
- Eligibility Check
- Benefits Inquiry
- Provider Lookup
- Pre Authorization Status
- Service Request
- Agent Escalation

## Core Entities

- member_id
- claim_id
- date_of_birth
- zip_code
- address
- ssn_last4
- plan_type
- provider_name
- claim_amount
- procedure_code

## Authentication Requirements

Users must be authenticated before accessing protected healthcare information.

Authentication may include:

- User ID
- Date of Birth
- ZIP Code
- Address Verification
- Last Four Digits of SSN

## Repository Structure

01_Pre_Requisites

Project requirements, scope, and compliance requirements.

02_Project_Overview

Project objective, problem statement, and solution overview.

03_Intent_and_Entity_Design

Intents, entities, and mappings.

04_Master_Conversational_Flow

High level conversational flow.

05_Welcome_and_Consent

Welcome and consent journeys.

06_Intent_Routing

Intent identification and routing.

07_Authentication_and_Verification

Authentication and verification flows.

08_Happy_Path_Journeys

Healthcare service journeys.

09_Escalation_and_Closure

Escalation and closure handling.

10_End_to_End_Flow

Complete conversational flow with edge cases.

11_Test_Data

Sample healthcare datasets.

12_Reference_Documents

Project requirement documents.
