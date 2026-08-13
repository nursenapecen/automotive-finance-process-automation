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

This Epic covers the creation, management, and validation of customer information required for financing applications. It aims to provide finance advisors with a centralized and standardized way to manage customer data.

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
FR-013

**Business Rules**

BR-CUS-001
BR-CUS-002
BR-CUS-006

**Description**

As a **Finance Advisor**,
**I want** to create a customer application by entering customer information into a centralized platform,
**so that** I can initiate the financing process without maintaining paper-based records.


**Business Value**

•	Eliminates paper-based application forms. 
•	Creates a standardized customer onboarding process. 
•	Reduces data entry errors. 
•	Enables downstream automation. 

**Dependencies**

None

**Acceptance Criteria**

See *Acceptance-Criteria.md* → AC-001

---

### US-002 – Update Customer Information

•	**Epic:** Customer Management 
•	**Feature:** Customer Registration 
•	**Priority:** Must Have 
•	**Story Points:** 3 
As a **Finance Advisor**,
**I want to** edit customer information before submitting the application,
**so that** incorrect or outdated information can be corrected.

---

### US-003 – Validate Mandatory Customer Information

•	**Epic:** Customer Management 
•	**Feature:** Customer Validation 
•	**Priority:** Must Have 
•	**Story Points:** 3 
As a **Finance Advisor**,
**I want to** validate customer information before submitting a financing application,
**so that** incomplete or incorrect customer data does not proceed to the financing institutions

---

### US-004 – Prevent Duplicate Applications

•	**Epic:** Customer Management 
•	**Feature:** Application Validation 
•	**Priority:** Should Have 
•	**Story Points:** 5 
As a **Finance Advisor**,
**I want to** be notified when a duplicate application exists,
**so that** I do not submit the same financing request multiple times.

---

# Epic 2 — Vehicle Management

## Feature: Vehicle Information

This Epic covers the management and validation of vehicle information required for financing applications, including vehicle type, invoice amount, and other relevant vehicle details.

### US-005 – Add Vehicle Information

**Epic**
Vehicle Management
**Feature**
Vehicle Information
**Priority**
Must Have
**Story Points**
5
**Related Business Requirement**
•	BR-004 
**Related Functional Requirements**
•	FR-015 
•	FR-016 
•	FR-018 
•	FR-021 
**Related Business Rules**
•	BR-VEH-001 
•	BR-VEH-003 
 
**User Story**
As a **Finance Advisor**,
**I want to** register the vehicle information for the financing application,
**so that** the financing request can be evaluated based on the selected vehicle.
 
**Business Value**
•	Ensures accurate financing calculations. 
•	Prevents inconsistent vehicle information. 
•	Enables automatic eligibility checks. 
 
**Dependencies**
US-001
 
**Acceptance Criteria**
See *Acceptance-Criteria.md* → AC-010

---

### US-006 – Select Vehicle Type

•	**Epic:** Vehicle Management 
•	**Feature:** Vehicle Validation 
•	**Priority:** Must Have 
•	**Story Points:** 3 
As a **Finance Advisor**,
**I want to** validate vehicle information before submitting a financing application,
**so that** the application contains accurate vehicle data.

---

### US-007 – Calculate Financing Amount

•	**Epic:** Vehicle Management 
•	**Feature:** Financing Calculation 
•	**Priority:** Must Have 
•	**Story Points:** 5 
As a **Finance Advisor**,
**I want to** calculate the requested financing amount based on vehicle and customer information,
**so that** I can prepare an accurate financing application.

---

# Epic 3 — Loan Application

## Feature: Loan Processing

This Epic covers the core financing application process, including finance institution selection, campaign selection, application review, submission, and receiving financing offers.

### US-008 – Select Finance Institutions

**Epic**
Loan Application
**Feature**
Finance Institution Selection
**Priority**
Must Have
**Story Points**
5
**Related Business Requirements**
•	BR-006 
**Related Functional Requirements**
•	FR-029 
•	FR-030 
•	FR-032 
**Related Business Rules**
•	BR-LOAN-001 
•	BR-FIN-001 
 
**User Story**
As a **Finance Advisor**,
**I want to** select one or more finance institutions for a financing application,
**so that** I can compare financing offers and provide the best option for the customer.
 
**Business Value**
•	Eliminates repetitive submissions. 
•	Supports multi-bank comparison. 
•	Reduces processing time. 
 
**Dependencies**
US-001
US-005
 
**Acceptance Criteria**
See *Acceptance-Criteria.md* → AC-018

---

### US-009 – Select Loan Campaign

•	**Epic:** Loan Application 
•	**Feature:** Campaign Management 
•	**Priority:** Should Have 
•	**Story Points:** 3 
As a **Finance Advisor**,
**I want to** select an applicable financing campaign,
**so that** the customer can receive the relevant financing conditions.

---

### US-010 – Review Loan Details

•	**Epic:** Loan Application 
•	**Feature:** Application Review 
•	**Priority:** Must Have 
•	**Story Points:** 3 
As a **Finance Advisor**,
**I want to** review all application information before submission,
**so that** I can verify the accuracy of the application.

---

### US-011 – Submit Loan Application

**Epic**
Loan Application
**Feature**
Loan Submission
**Priority**
Must Have
**Story Points**
8

**Business Requirement**
BR-008

**Functional Requirements**
FR-033
FR-034
FR-037
FR-041

**Business Rules**
BR-LOAN-001
BR-LOAN-004
BR-RPA-001

**Description**
As a **Finance Advisor**
**I want to** submit a completed loan application to one or more finance institutions
**So that** the customer can receive financing offers without manually entering data into multiple bank portals.

**Business Value**
•	Eliminates duplicate data entry 
•	Reduces application processing time 
•	Standardizes financing workflow 
•	Improves advisor productivity 

Dependencies
•	US-001 
•	US-005 
•	US-008 
•	US-010 

**Acceptance Criteria**
See *Acceptance-Criteria.md* -> AC-011

**Notes**
Application submission initiates the RPA automation workflow.

---

### US-012 – Receive Loan Response

•	**Epic:** Loan Application 
•	**Feature:** Financing Response 
•	**Priority:** Must Have 
•	**Story Points:** 5
As a **Finance Advisor**,
**I want to** receive financing offers and application results from the selected finance institutions in the centralized platform,
**so that** I can review the available financing options without checking each finance institution's portal separately.

---

# Epic 4 — OCR Processing

This Epic focuses on digitizing customer information from paper-based documents using OCR technology. It aims to reduce manual data entry and improve the accuracy and efficiency of customer data collection.

### US-013 – Upload Customer Documents

•	**Epic:** OCR Processing 
•	**Feature:** Document Management 
•	**Priority:** Must Have 
•	**Story Points:** 5 
As a **Finance Advisor**,
**I want to** upload customer documents to the financing platform,
**so that** the required information can be processed digitally.

---

### US-014 – Extract Customer Information Using OCR

**Epic**
OCR Processing

**Feature**
Document Processing

**Priority**
Must Have

**Story Points**
8

**Related Business Requirements**
•	BR-009 

**Related Functional Requirements**
•	FR-022 
•	FR-023 
•	FR-024 
•	FR-026 

**Related Business Rules**
•	BR-OCR-001 
•	BR-OCR-002 
•	BR-OCR-003 
 
**User Story**
As a **Finance Advisor**,
**I want to** automatically extract customer information from uploaded identity documents,
**so that** I do not need to manually enter the same information into the application.
 
**Business Value**
•	Reducing manual effort. 
•	Improving data accuracy. 
•	Accelerates application creation. 
•	Supports digital document management. 
 
**Dependencies**
US-013
 
**Acceptance Criteria**
See *Acceptance-Criteria.md* → AC-031

---

### US-015 – Validate OCR Results

•	**Epic:** OCR Processing 
•	**Feature:** OCR Validation 
•	**Priority:** Must Have 
•	**Story Points:** 5 
As a **Finance Advisor**,
**I want to** review and correct OCR-extracted customer information,
**so that** the financing application contains accurate customer data.

---

# Epic 5 — Finance Institution Integration

This Epic covers the exchange of financing application data and responses between the centralized platform and selected finance institutions, enabling advisors to manage multiple applications through a single process.

### US-016 – Send Application to Finance Institutions

•	**Epic:** Finance Institution Integration 
•	**Feature:** Application Submission 
•	**Priority:** Must Have 
•	**Story Points:** 8 
As a **Finance Advisor**,
**I want to** send a completed financing application to the selected finance institutions,
**so that** I can obtain financing offers without manually entering the information into each portal.

---

### US-017 – Receive Finance Institution Responses

•	**Epic:** Finance Institution Integration 
•	**Feature:** Application Response 
•	**Priority:** Must Have 
•	**Story Points:** 5 
As a **Finance Advisor**,
**I want to** receive financing responses in the centralized platform,
**so that** I can review the available offers without checking each finance institution portal separately.

---

### US-018 – Retry Failed Integrations

•	**Epic:** Finance Institution Integration 
•	**Feature:** Integration Exception Handling 
•	**Priority:** Could Have 
•	**Story Points:** 5 
As a **Finance Advisor**,
**I want to** retry a failed finance institution submission,
**so that** temporary integration failures do not require the entire application to be processed manually.

---

# Epic 6 — RPA Automation

This Epic focuses on automating repetitive data entry and application submission activities across finance institution portals using RPA technology. It aims to reduce manual effort and accelerate the financing process.

### US-019 – Trigger RPA

**Epic**
RPA Automation
**Feature**
Application Submission
**Priority**
Must Have
**Story Points**
8

**Related Business Requirements**
•	BR-010 

**Related Functional Requirements**
•	FR-041 
•	FR-042 
•	FR-046 
•	FR-048 

**Related Business Rules**
•	BR-RPA-001 
•	BR-RPA-003 
•	BR-RPA-005 
 
**User Story**
As a **Finance Advisor**,
**I want to** automatically submit financing applications to selected finance institutions,
**so that** I no longer need to manually enter the same application into multiple external systems.
 
**Business Value**
•	Eliminates repetitive manual work. 
•	Standardizes application submission. 
•	Reduces operational costs. 
•	Minimizes human error. 
 
**Dependencies**
US-011
US-014
 
**Acceptance Criteria**
See *Acceptance-Criteria.md* → AC-041

---

### US-020 – Enter OTP

•	**Epic:** RPA Automation 
•	**Feature:** OTP / SMS Verification 
•	**Priority:** Must Have 
•	**Story Points:** 5 
As a **Finance Advisor**,
**I want to** enter the customer SMS verification code when requested by the finance institution,
**so that** the RPA process can continue and complete the financing application.

---

### US-021 – Complete Automated Submission

•	**Epic:** RPA Automation 
•	**Feature:** Automated Data Entry 
•	**Priority:** Must Have 
•	**Story Points:** 8 
As a **Finance Advisor**,
**I want to** have validated application data automatically entered into finance institution portals,
**so that** repetitive manual data entry is eliminated.

---

### US-022 – Handle Failed RPA Executions

•	**Epic:** RPA Automation 
•	**Feature:** Exception Handling 
•	**Priority:** Should Have 
•	**Story Points:** 5 
As a **Finance Advisor**,
**I want to** be informed when an automated submission fails,
**so that** I can take the necessary corrective action.

---

# Epic 7 — Application Tracking

This Epic provides finance advisors with centralized visibility into financing application statuses and histories, allowing them to monitor progress and identify applications requiring further action.

### US-023 – View Application Status

**Epic**
Application Tracking
**Feature**
Application Monitoring
**Priority**
Must Have
**Story Points**
5

**Related Business Requirements**
•	BR-011 

**Related Functional Requirements**
•	FR-051 
•	FR-052 
•	FR-055 

**Related Business Rules**
•	BR-LOAN-005 
•	BR-REP-001 
 
**User Story**
As a **Finance Advisor**,
**I want to** monitor the status of all financing applications from a centralized dashboard,
**so that** I can quickly identify pending actions and keep customers informed about their application progress.
 
**Business Value**
•	Improves operational visibility. 
•	Reduces time spent checking multiple finance institution portals. 
•	Enhances customer communication. 
•	Enables faster issue resolution. 
 
**Dependencies**
US-019
 
**Acceptance Criteria**
See *Acceptance-Criteria.md* → AC-050

---

### US-024 – View Application History

•	**Epic:** Application Tracking 
•	**Feature:** Application History 
•	**Priority:** Should Have 
•	**Story Points:** 3 
As a **Finance Advisor**,
**I want to** view the history of a financing application,
**so that** I can understand previous actions and status changes.

---

### US-025 – Search Applications

•	**Epic:** Application Tracking 
•	**Feature:** Application Search 
•	**Priority:** Should Have 
•	**Story Points:** 3 
As a **Finance Advisor**,
**I want to** search financing applications using customer or application information,
**so that** I can quickly find the application I need.

---

# Epic 8 — Reporting

This Epic provides centralized reporting and monitoring capabilities for financing applications, enabling users to analyze application activity and operational performance.

### US-026 – Generate Application Report

**Epic**
Reporting
**Feature**
Application Dashboard
**Priority**
Should Have
**Story Points**
5

**Related Business Requirements**
•	BR-011

**Related Functional Requirements**
•	FR-056
•	FR-057
•	FR-058
•	FR-059
•	FR-061

**Related Business Rules**
•	BR-REP-001
•	BR-REP-002
•	BR-REP-003
•	BR-REP-004
 
**User Story**
As a **Finance Advisor**,
**I want to** view financing applications and related operational performance information through a centralized dashboard,
**so that** I can monitor application activity, identify pending or completed applications, and evaluate the status of the financing process without checking multiple sources separately.
 
**Business Value**
•	Provides centralized visibility into financing application activities.
•	Reduces the need to manually track applications across different sources.
•	Enables faster identification of pending or completed applications.
•	Supports operational performance monitoring.
•	Helps finance advisors manage customer financing requests more efficiently.
 
**Dependencies**
•	US-011 – Submit Loan Application
•	US-012 – Receive Financing Offers
•	US-023 – Track Application Status
 
Acceptance Criteria
See *Acceptance-Criteria.md* → AC-026

---

### US-027 – Filter Reports

•	**Epic:** Reporting 
•	**Feature:** Report Filtering 
•	**Priority:** Should Have 
•	**Story Points:** 3 
As a **Finance Manager**,
**I want to** filter financing reports by relevant criteria,
**so that** I can analyze application activity and operational performance.

---

### US-028 – Export Reports

•	**Epic:** Reporting 
•	**Feature:** Report Export 
•	**Priority:** Could Have 
•	**Story Points:** 3 
As a **Finance Manager**,
**I want to** export financing reports,
**so that** I can perform further analysis and share results with relevant stakeholders.

---

# Epic 9 — Notifications

This Epic covers notifications related to financing application status changes, missing information, and application results, helping advisors and customers stay informed throughout the process.

### US-029 – Notify Finance Advisor

•	**Epic:** Notifications 
•	**Feature:** Advisor Notifications 
•	**Priority:** Should Have 
•	**Story Points:** 3 
As a **Finance Advisor**,
**I want to** receive notifications when an application status changes,
**so that** I can take the required next action and keep the customer informed.

---

### US-030 – Notify Customer

•	**Epic:** Notifications 
•	**Feature:** Customer Notifications 
•	**Priority:** Should Have 
•	**Story Points:** 3 
As a **Customer**,
**I want to** receive notifications about my financing application,
**so that** I can stay informed about the progress of my application.

---

## Story Dependencies

| Story  | Depends On |
| ------ | ---------- |
| US-002 | US-001     |
| US-003 | US-001     |
| US-005 | US-001     |
| US-006 | US-005     |
| US-007 | US-005     |
| US-008 | US-005     |
| US-009 | US-008     |
| US-010 | US-003     |
| US-011 | US-010     |
| US-012 | US-011     |
| US-013 | US-001     |
| US-014 | US-013     |
| US-015 | US-014     |
| US-016 | US-011     |
| US-017 | US-016     |
| US-018 | US-016     |
| US-019 | US-011     |
| US-020 | US-019     |
| US-021 | US-020     |
| US-022 | US-019     |
| US-023 | US-019     |
| US-024 | US-023     |
| US-025 | US-001     |
| US-026 | US-023     |
| US-027 | US-026     |
| US-028 | US-026     |
| US-029 | US-023     |
| US-030 | US-012     |

---

## Story Traceability

| Story  | BR     | FR     | Rule        | AC     |
| ------ | ------ | ------ | ----------- | ------ |
| US-001 | BR-001 | FR-006 | BR-CUS-001  | AC-001 |
| US-002 | BR-001 | FR-012 | BR-CUS-006  | AC-004 |
| US-003 | BR-001 | FR-013 | BR-CUS-006  | AC-007 |
| US-004 | BR-001 | FR-014 | BR-CUS-003  | AC-010 | 
| US-005 | BR-003 | FR-015 | BR-VEH-001  | AC-011 |
| US-006 | BR-003 | FR-021 | BR-VEH-003  | AC-014 |
| US-007 | BR-003 | FR-018 | BR-VEH-003  | AC-017 |
| US-008 | BR-004 | FR-029 | BR-LOAN-001 | AC-020 |
| US-009 | BR-007 | FR-037 | BR-CMP-002  | AC-023 |
| US-010 | BR-008 | FR-040 | BR-LOAN-004 | AC-026 |
| US-011 | BR-008 | FR-046 | BR-LOAN-002 | AC-029 |
| US-012 | BR-008 | FR-048 | BR-LOAN-005 | AC-032 |
| US-013 | BR-004 | FR-022 | BR-OCR-001  | AC-035 |
| US-014 | BR-004 | FR-023 | BR-OCR-001  | AC-038 |
| US-015 | BR-004 | FR-026 | BR-OCR-003  | AC-041 |
| US-016 | BR-010 | FR-046 | BR-FIN-002  | AC-044 |
| US-017 | BR-010 | FR-047 | BR-FIN-003  | AC-047 |
| US-018 | BR-010 | FR-049 | BR-RPA-006  | AC-050 |
| US-019 | BR-010 | FR-041 | BR-RPA-001  | AC-053 |
| US-020 | BR-010 | FR-042 | BR-RPA-003  | AC-056 |
| US-021 | BR-010 | FR-046 | BR-RPA-004  | AC-059 |
| US-022 | BR-010 | FR-049 | BR-RPA-005  | AC-062 | 
| US-023 | BR-011 | FR-051 | BR-LOAN-005 | AC-065 |
| US-024 | BR-011 | FR-055 | BR-REP-004  | AC-068 |
| US-025 | BR-011 | FR-056 | BR-REP-001  | AC-071 |
| US-026 | BR-011 | FR-056 | BR-REP-002  | AC-074 |
| US-027 | BR-011 | FR-057 | BR-REP-003  | AC-077 |
| US-028 | BR-011 | FR-060 | BR-REP-004  | AC-080 |
| US-029 | BR-012 | FR-062 | BR-NOT-002  | AC-083 |
| US-030 | BR-012 | FR-063 | BR-NOT-001  | AC-086 |

