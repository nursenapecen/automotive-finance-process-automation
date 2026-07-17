# 🚗 Automotive Finance Process Automation

> **Business Analysis Case Study**
>
> Digital transformation of the automotive financing process using **OCR** and **Robotic Process Automation (RPA)**.

---

## Table of Contents

- Project Overview
- Business Problem
- Project Objectives
- Existing Process (As-Is)
- Future Process (To-Be)
- Proposed Solution
- Business Value
- Scope
- Stakeholders
- My Role
- Project Deliverables
- Repository Structure
- Technologies
- Future Improvements

---

## 📚 Project Documents

| Document | Description |
|----------|-------------|
| [Business Requirements](docs/business-requirements.md) | Business objectives and scope |
| [Functional Requirements](docs/functional-requirements.md) | Detailed functional requirements |
| [Business Rules](docs/business-rules.md) | Business rules |
| [Stakeholder Analysis](docs/stakeholder-analysis.md) | Stakeholder overview |
| [Process Overview](docs/process-overview.md) | As-Is and To-Be processes |

# Project Overview

## Background

When customers purchase a new or used vehicle, they often apply for vehicle financing through one of several contracted finance institutions.

In the current process, finance advisors manually collect customer information from multiple physical documents and repeatedly enter identical information into each finance institution's application portal.

This repetitive process increases operational workload, prolongs financing decisions, and negatively impacts customer experience.

This case study demonstrates how the financing application process can be redesigned using Business Analysis techniques together with OCR and Robotic Process Automation.

---

# Business Problem

## Current Challenges

Finance advisors experience several operational challenges during financing applications:

- Customer information exists across multiple physical documents.
- There is no centralized application screen.
- The same customer information must be entered repeatedly into different finance company portals.
- Manual data entry increases processing time.
- Manual work increases the possibility of human error.
- Customers wait longer to receive financing offers.
- Advisors spend significant time on repetitive administrative tasks instead of customer interaction.

---

#  Project Objectives

The project aims to:

 Create a centralized finance application screen

 Collect all customer information in one place

 Extract information from documents using OCR

 Automatically submit applications via RPA

 Eliminate repetitive manual data entry

 Improve operational efficiency

 Reduce processing time

 Improve customer experience

---

#  Existing Process (As-Is)

Current financing process:

```text
Customer

↓

Provides Documents

↓

Finance Advisor

↓

Collect Customer Information

↓

Finance Company Portal A

↓

Manual Data Entry

↓

Finance Company Portal B

↓

Manual Data Entry

↓

Finance Company Portal C

↓

Manual Data Entry

↓

Receive Financing Offers
```

### Pain Points

- Multiple manual entries
- Long processing time
- High workload
- Risk of inconsistent information
- No centralized data source

---

#  Future Process (To-Be)

Proposed future process:

```text
Customer

↓

Provide Documents

↓

OCR

↓

Central Finance Application Screen

↓

Advisor Validation

↓

RPA

↓

Finance Company A

↓

Finance Company B

↓

Finance Company C

↓

Loan Offers

↓

Customer
```

---

#  Proposed Solution

The proposed solution consists of three major components.

## 1. Centralized Finance Application Screen

A single application screen where finance advisors manage all customer and vehicle information.

---

## 2. OCR Integration

Customer documents are scanned automatically.

OCR extracts information such as:

- Identity Information
- Address
- Occupation
- Income
- Contact Details
- Vehicle Information

---

## 3. Robotic Process Automation

After verification by the advisor, an RPA bot automatically submits customer information to selected finance institutions.

The advisor no longer needs to enter identical information multiple times.

---

# Expected Business Value

| Business Value | Benefit |
|---------------|---------|
| Operational Efficiency | Reduces repetitive manual work |
| Faster Processing | Shortens financing application time |
| Better Customer Experience | Customers receive offers faster |
| Data Quality | Reduces manual entry errors |
| Standardization | One unified application process |
| Digital Transformation | Supports automation initiatives |

---

#  Project Scope

## In Scope

- Customer Information Collection
- Vehicle Information
- OCR Integration
- RPA Automation
- Finance Institution Selection
- Financing Application

---

## Out of Scope

- Credit Approval Decision
- Bank Internal Processes
- Payment Operations
- Contract Generation

---

#  Stakeholders

| Stakeholder | Responsibility |
|-------------|---------------|
| Customer | Applies for financing |
| Finance Advisor | Collects and validates customer information |
| Finance Institutions | Evaluate financing applications |
| Business Analyst | Requirement analysis |
| RPA Team | Process automation |
| OCR Team | Document extraction |
| Development Team | Application development |

---

#  My Role

As the Business Analyst, I was responsible for:

- Business Process Analysis
- Requirement Gathering
- Stakeholder Communication
- Process Mapping
- Functional Requirement Definition
- User Story Creation
- Acceptance Criteria
- Wireframe Design
- BPMN Modeling
- Process Improvement Analysis

---

#  Project Deliverables

This repository contains:

- Business Requirements Document
- Functional Requirements
- Business Rules
- User Stories
- Acceptance Criteria
- BPMN Diagrams
- As-Is Process
- To-Be Process
- Wireframes
- Solution Architecture

---

#  Repository Structure

```text
automotive-finance-process-automation

│
├── README.md
│
├── docs
│   ├── Business-Requirements.md
│   ├── Functional-Requirements.md
│   ├── User-Stories.md
│   ├── Acceptance-Criteria.md
│   ├── Business-Rules.md
│
├── diagrams
│   ├── as-is-process.png
│   ├── to-be-process.png
│   ├── solution-architecture.png
│
├── wireframes
│   ├── finance-application-screen.png
│
└── images
```

---

#  Technologies & Methodologies

### Business Analysis

- Business Process Analysis
- Requirement Engineering
- Gap Analysis
- Process Improvement
- BPMN
- UML

### Tools

- Visio
- Draw.io
- Figma
- Jira
- Miro

### Technologies

- OCR
- Robotic Process Automation (RPA)

---

#  Success Metrics

Expected improvements:

- Reduced manual data entry
- Faster financing applications
- Improved advisor productivity
- Reduced processing errors
- Improved customer satisfaction
- Standardized financing process

---

#  Future Improvements

Possible future enhancements include:

- Digital document upload by customers
- AI-assisted document validation
- API integration with finance institutions
- Automatic eligibility scoring
- Real-time financing comparison
- Digital signature integration

---

#  Related Documents

Coming soon:

- Business Requirements
- Functional Requirements
- User Stories
- Acceptance Criteria
- Wireframes
- BPMN Diagrams

---

#  About This Repository

This repository is part of my Business Analysis portfolio and demonstrates how business analysis techniques can be applied to redesign and automate manual business processes in the automotive finance domain.

The focus of this project is not software development, but business process analysis, requirements engineering, and digital transformation.

---

## 📬 Contact

**Nursena Peçen**

Business Analyst | Product Owner

LinkedIn: (https://www.linkedin.com/in/nursena-pecen/)

GitHub: https://github.com/nursenapecen
