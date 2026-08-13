# Business Requirements

## Executive Summary

This project focuses on digitizing the automotive financing application process.

Currently, finance advisors manually enter the same customer information into multiple financial institution portals.

The proposed solution introduces a centralized financing platform supported by OCR and RPA automation to eliminate repetitive data entry, improve operational efficiency, and reduce customer waiting time.


## Business Context 

Automotive dealerships collaborate with multiple financing institutions.

Each institution requires customer information through separate portals.

As a result

-same data

-same documents

-same verification

-same workflow

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

•	Reduce manual work

•	Improve operational efficiency

•	Increase customer satisfaction

•	Reduce application processing time

•	Provide centralized monitoring

•	Support future API integrations


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

•	Customer Information
•	Vehicle Information
•	Loan Applications
•	OCR
•	RPA
•	Tracking
•	Reporting

### Out Scope

•	Credit approval decision
•	Risk scoring
•	Bank internal processes
•	Loan payment


## Business Requirements

### BR-001 – Centralized Financing Application

The financing application process shall be managed through a centralized interface, enabling finance advisors to manage customer and application information without relying on multiple disconnected sources.

### BR-002 – Customer Information Management

The solution shall provide a standardized way to capture, manage, and validate the customer information required for financing applications.

### BR-003 – Vehicle Information Management

The solution shall support the management of the vehicle information required for financing applications, including brand, model, variant, year, and color.

### BR-004 – Financing Institution Management

The solution shall support applications to multiple partnered finance institutions through a centralized financing process.

### BR-005 – Digital Document Processing

The solution shall digitize customer information from paper-based documents to reduce manual data entry and improve data availability.

### BR-006 – Automated Data Extraction

The solution shall use OCR technology to extract relevant customer information from uploaded documents and reduce repetitive manual data entry.

### BR-007 – Financing Application Validation

The financing process shall ensure that customer, vehicle, and application information is complete and accurate before an application is submitted to a finance institution.

### BR-008 – Financing Offer Management

The solution shall enable finance advisors to receive and review financing offers and application results from selected finance institutions through a centralized interface.

### BR-009 – Process Automation

The financing application process shall minimize repetitive manual activities by using RPA to transfer validated application information to finance institution portals.

### BR-010 – Application Tracking

The solution shall provide centralized visibility into financing application statuses and histories throughout the application process.

### BR-011 – Operational Reporting

The solution shall provide reporting and monitoring capabilities to support the analysis of financing applications and operational performance.

### BR-012 – Notifications and Alerts

The solution shall provide timely notifications and alerts regarding application status changes, missing information, and relevant process events.

### BR-013 – Operational Efficiency

The solution shall reduce manual processing effort and financing application processing time while improving the productivity of finance advisors.

### BR-014 – Customer Experience

The solution shall reduce customer waiting time and improve the overall financing experience by accelerating the application and offer retrieval process.

## Business Rule

*The detailed business rules are provided in the business-rules.md document.


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

Paper-based Data

↓

OCR

↓

ERP

↓

RPA

↓

Financial Institution

↓

RPA
↓

ERP

↓

Notification


## Integration Landscape

The detailed integration landscape are provided in the integration-landscape.md diagram.

OCR

↓

ERP

↓

RPA

↓

Bank A

Bank B

Bank C

↓

Email Notification Service

↓

Reporting


## Risks

| Risk           | Mitigation        |
| -------------- | ----------------- |
| Portal changes | Update bot        |
| OCR errors     | Manual validation |
| OTP timeout    | Retry             |
| Bank downtime  | Queue             |


