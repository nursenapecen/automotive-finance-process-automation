
## Executive Summary

This project focuses on digitizing the automotive financing application process.

Currently, finance advisors manually enter the same customer information into multiple financial institution portals.

The proposed solution introduces a centralized financing platform supported by OCR and RPA automation to eliminate repetitive data entry, improve operational efficiency, and reduce customer waiting time.


## Business Context 

Automotive dealerships collaborate with multiple financing institutions.

Each institution requires customer information through separate portals.

As a result

same data

same documents

same verification

same workflow

must be repeated several times.


## Current Business Process (As-Is)

Customer

↓

Finance Advisor

↓

Manual Data Entry into ERP

↓

Financial Instution Portal 1

↓

Financial Instution Portal 2

↓

Financial Instution Portal 3

↓

Wait

↓

Manual Tracking

↓

Customer


## Pain Points

| Pain Point | Impact |
| --- | --- |
| Duplicate Data Entry | High |
| Manuel Document Upload | High |
| Data Loss | High |
| Multiple Bank Portal | Medium |
| Human Erros | High |
| Long customer waiting time | High |
| Difficult Tracking | Medium |


## Business Objectives

Reduce manual work

Improve operational efficiency

Increase customer satisfaction

Reduce application processing time

Provide centralized monitoring

Support future API integrations


## Success Metrics

| Metric | Current | Target |
| --- | --- | --- |
| Montly Loan Apllication | 2500 | 2500 |
| Manual Effort | 39h | 19h |
| Manual Work Ratio | 25% | 12% |
| Annual Saving | - | 90.5K € |


## Stakeholders

| Stakeholder            | Responsibility       |
| ---------------------- | -------------------- |
| Customer               | Provides information |
| Finance Advisor        | Loan application     |
| Product Owner          | Product vision       |
| Business Analyst       | Requirements         |
| RPA Team               | Automation           |
| OCR Service            | Document extraction  |
| Financial Institutions | Credit evaluation    |


## Scope 

### In Scope 

Customer Information
Vehicle Information
Loan Applications
OCR
RPA
Tracking
Reporting

### Out Scope

Credit approval decision
Risk scoring
Bank internal processes
Loan payment


## Business Requirements

BR-001

The system shall allow advisors to create financing applications from a single interface.

BR-002

The system shall create unique Application ID.

BR-003

The system shall support multiple financial institutions.

BR-004

The system shall automatically populate customer information using OCR.

BR-005

The system shall trigger RPA after advisor confirmation.

BR-006

The system shall track application status.

BR-007

The system shall trigger automatic system alerts.


## Business Rule

*The detailed business rules are provided in the business-rules.md document.

BRULE-001

Customer ID is mandatory.

BRULE-002

Only Financial Advisors may approve applications.

BRULE-003

Approval is permitted only when all mandatory documents have been submitted.

BRULE-004

OTP verification is required.

BRULE-005

OCR fields remain editable.

BRULE-006

Financial Instituion selection is mandatory.


## Functional Requirements Categories

*The detailed functional requirements are provided in the functional-requirements.md document.

-Authentication
-Customer
-Vehicle
-Credit
-Documents
-Reporting
-Notifications


## Non Functional Requirements

| Category     | Requirement     |
| ------------ | --------------- |
| Availability | 99%             |
| Security     | GDPR            |
| Performance  | <3 sec          |
| Logging      | All bot actions |
| Audit        | Full history    |
| Scalability  | New banks       |


## Process Automation 

ERP

↓

OCR

↓

RPA

↓

Financial Institution

↓

OCR

↓

ERP

↓

Notification


## Integration Landscape

The detailed integration landscape are provided in the integration-landscape.md diagram.

ERP

↓

OCR

↓

RPA

↓

Bank A

Bank B

Bank C

↓

Email Service

↓

Reporting


## Risks

| Risk           | Mitigation        |
| -------------- | ----------------- |
| Portal changes | Update bot        |
| OCR errors     | Manual validation |
| OTP timeout    | Retry             |
| Bank downtime  | Queue             |


## Traceability Matrix 

| Objective          | BR     | User Story | Test  |
| ------------------ | ------ | ---------- | ----- |
| Reduce manual work | BR-001 | US-01      | TC-01 |
| Faster processing  | BR-005 | US-06      | TC-10 |


