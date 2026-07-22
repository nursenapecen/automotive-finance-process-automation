# User Stories

## 1. Document Overview

This document defines the Product Backlog for the Automotive Finance Process Automation project.

The backlog is organized into Epics and Features, providing traceability between Business Requirements, Functional Requirements, Business Rules, Acceptance Criteria, and Test Cases.

---

## 2. Story Prioritization

| Priority | Description |
|----------|-------------|
| Must Have | Required for MVP |
| Should Have | Important but not mandatory |
| Could Have | Nice to have |
| Won't Have | Planned for future releases |

---

## 3. Story Point Scale

| Story Points | Complexity |
|--------------|------------|
| 1 | Very Small |
| 2 | Small |
| 3 | Medium |
| 5 | Large |
| 8 | Very Large |
| 13 | Complex |

---

# Epic 1 — Customer Management

## Feature: Customer Registration

---

### US-001 – Create Customer Application

**Epic**

Customer Management

**Feature**

Customer Registration

**Priority**

Must Have

**Story Points**

5

**Business Requirement**

BR-001

**Functional Requirements**

FR-006
FR-007
FR-008
FR-009

**Business Rules**

BR-CUS-001
BR-CUS-002
BR-CUS-006

**Description**

As a Finance Advisor,

I want to create a customer application,

so that I can initiate the financing process.

**Business Value**

Reduces manual paperwork and standardizes customer onboarding.

**Dependencies**

None

**Acceptance Criteria**

See AC-001

---

### US-002 – Update Customer Information

...

---

### US-003 – Validate Mandatory Customer Information

...

---

### US-004 – Prevent Duplicate Applications

...

---

# Epic 2 — Vehicle Management

## Feature: Vehicle Information

---

### US-005 – Add Vehicle Information

...

---

### US-006 – Select Vehicle Type

...

---

### US-007 – Calculate Financing Amount

...

---

# Epic 3 — Loan Application

## Feature: Loan Processing

---

### US-008 – Select Finance Institutions

...

---

### US-009 – Select Loan Campaign

...

---

### US-010 – Review Loan Details

...

---

### US-011 – Submit Loan Application

...

---

### US-012 – Receive Loan Response

...

---

# Epic 4 — OCR Processing

---

### US-013 – Upload Customer Documents

...

---

### US-014 – Extract Customer Information Using OCR

...

---

### US-015 – Validate OCR Results

...

---

# Epic 5 — Finance Institution Integration

---

### US-016 – Send Application to Finance Institutions

...

---

### US-017 – Receive Finance Institution Responses

...

---

### US-018 – Retry Failed Integrations

...

---

# Epic 6 — RPA Automation

---

### US-019 – Trigger RPA

...

---

### US-020 – Enter OTP

...

---

### US-021 – Complete Automated Submission

...

---

### US-022 – Handle Failed RPA Executions

...

---

# Epic 7 — Application Tracking

---

### US-023 – View Application Status

...

---

### US-024 – View Application History

...

---

### US-025 – Search Applications

...

---

# Epic 8 — Reporting

---

### US-026 – Generate Application Report

...

---

### US-027 – Filter Reports

...

---

### US-028 – Export Reports

...

---

# Epic 9 — Notifications

---

### US-029 – Notify Finance Advisor

...

---

### US-030 – Notify Customer

...

---

## Story Dependencies

| Story | Depends On |
|---------|------------|
| US-005 | US-001 |
| US-008 | US-005 |
| US-011 | US-008 |
| US-014 | US-013 |
| US-019 | US-011 |
| US-023 | US-019 |

---

## MVP Scope

### Must Have

US-001 → US-023

### Should Have

US-024 → US-028

### Could Have

US-029
US-030

---

## Story Traceability

| Story | BR | FR | Rule | AC | TC |
|---------|------|------|------|------|------|
| US-001 | BR-001 | FR-006 | BR-CUS-001 | AC-001 | TC-001 |
| US-002 | BR-001 | FR-012 | BR-CUS-006 | AC-004 | TC-004 |
| US-005 | BR-003 | FR-015 | BR-VEH-001 | AC-011 | TC-011 |
| US-011 | BR-008 | FR-046 | BR-LOAN-002 | AC-025 | TC-027 |
| US-019 | BR-010 | FR-041 | BR-RPA-001 | AC-039 | TC-044 |

