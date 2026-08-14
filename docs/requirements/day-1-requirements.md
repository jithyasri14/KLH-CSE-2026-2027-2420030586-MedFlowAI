# Day 1 Requirements Baseline

## Problem Statement

Fragmented healthcare information, manual coordination, inefficient appointments and queues, difficult-to-interpret documents, delayed communication, and emergency workflow delays create a need for a secure and intelligent coordination platform.

## Objectives

- Connect core healthcare workflows through clear service boundaries.
- Provide least-privilege, role-based access.
- Demonstrate governed specialized AI assistants.
- Plan testable, observable, secure, and independently deployable components.
- Produce traceable Agile and GitHub evidence.

## Initial Functional Requirements

1. The system will authenticate users and enforce JWT/RBAC permissions.
2. Authorized users will manage patient, doctor, appointment, and medical-record workflows.
3. Supporting services will manage laboratory, pharmacy, billing, notification, and emergency workflows progressively.
4. The gateway will route protected REST APIs and services will register with Eureka.
5. The AI Service will coordinate planned assistants through Spring AI and Gemini.
6. Sensitive AI outputs will require human review and will not directly diagnose or prescribe.
7. The platform will record security-relevant and workflow audit events.

## Non-Functional Requirements

- Security: encrypted transport, secret protection, least privilege, input validation, and auditability.
- Privacy: synthetic data only; no real patient or institutional confidential information.
- Maintainability: modular services, documented APIs, progressive commits, and reviewed decisions.
- Scalability: independently scalable services where justified.
- Reliability: timeouts, controlled errors, idempotency where required, and AI fallback behavior.
- Observability: health, request, latency, error, and availability metrics.
- Testability: unit, integration, API, security, AI-evaluation, end-to-end, and performance tests.

## User Roles

Patient, Doctor, Nurse, Receptionist, Laboratory Staff, Pharmacist, Billing Staff, Emergency Staff, and Administrator.

## Major Workflows

- Registration, authentication, and role authorization
- Patient profile and authorized medical-history access
- Doctor availability, appointment booking, cancellation, rescheduling, and queue handling
- Clinical notes, prescriptions, laboratory requests, and reports
- Pharmacy verification, inventory insight, and dispensing
- Billing generation, status, viewing, and explanation
- Emergency intake, priority support, and staff notification
- AI-assisted summaries, guidance, explanations, and operational insights with human oversight

## Initial User Stories

- As a patient, I want to book an available appointment so that I can access care efficiently.
- As a doctor, I want authorized patient information organized in one view so that I can review it efficiently.
- As a receptionist, I want to manage appointments and queues so that patient flow is visible.
- As emergency staff, I want structured emergency information and alerts so that urgent workflows begin promptly.
- As a doctor, I want an AI-generated draft summary with sources so that I can review it rather than recreate it manually.
- As an administrator, I want service-health information so that operational problems are visible.

## Constraints

- Approximately 15 days for the first complete academic version.
- No real patient data, confidential institutional data, or committed credentials.
- No autonomous diagnosis, prescribing, or treatment.
- The project must demonstrate microservices without creating an unfinishable service estate.
- AWS deployment is conditional on time, cost, and academic value.

## Assumptions

- Team members will supply missing IDs and use their own GitHub accounts.
- The supervisor and coordinator will receive repository access.
- Local development tools and Gemini access will be verified later.
- Synthetic data will be sufficient for the academic demonstration.

