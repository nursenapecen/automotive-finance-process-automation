# Acceptance Criteria

## 1. Document Overview

This document defines the acceptance criteria for the key user stories of the Automotive Finance Process Automation project.

The acceptance criteria describe the conditions that must be satisfied for a user story to be considered complete and accepted.

The criteria are written using the Given / When / Then format to provide a common understanding between Business Analysts, Product Owners, Developers, and QA teams.

---

## 2. Acceptance Criteria Standards

The following structure is used throughout this document:

- **Given** – Defines the initial context or precondition.
- **When** – Defines the user action or system event.
- **Then** – Defines the expected outcomes.

Each acceptance criteria is uniquely identified using an AC ID.

---

# 3. Customer Management

## US-001 – Create Customer Application

### AC-001 – Create a New Application

**Given** the Finance Advisor is logged into the financing platform,

**When** the advisor starts a new finance application,

**Then** the system shall create a new application and allow the advisor to enter customer information.

---

### AC-002 – Enter Customer Information

**Given** a financing application has been created,

**When** the Finance Advisor enters the required customer information,

**Then** the system shall store the entered information in the application.

---

### AC-003 – Save Customer Application

**Given** the required customer informaiton has been entered,

**When** the Finance Advisor saves the application,

**Then** the system shall save the application and make it available for further processing.

---

## US-003 – Validate Customer Information

### AC-004 – Validate Mandatory Information

**Given** a financing application contains customer information,

**When** the Finance Advisor proceeds to the next step,

**Then** the system shall validate whether all mandatory customer information has been completed.

---

### AC-005 – Display Validation Errors

**Given** one or more mandatory customer fields are incomplete,

**When** the Finance Advisor attempts to proceed,

**Then** the system shall display the relevant validation message alarms.

---

### AC-006 – Prevent Invalid Submission

**Given** mandatory customer information is missing or invalid,

**When** the Finance Advisor attempts to submit the application,

**Then** the system shall prevent the application from proceeding until the required information is entered.

---

# 4. Vehicle Management

## US-005 – Add Vehicle Information

### AC-007 – Enter Vehicle Information

**Given** a financing application has been created,

**When** the Finance Advisor enters the vehicle information,

**Then** the system shall store the vehicle information within the application.

---

### AC-008 – Support Required Vehicle Information

**Given** the Finance Advisor is entering vehicle information,

**When** the vehicle information is provided,

**Then** the system shall support the required vehicle attributes, including brand, model, variant, year, and color.

---

### AC-009 – Associate Vehicle with Application

**Given** a financing application exists,

**When** the Finance Advisor adds vehicle information,

**Then** the vehicle information shall be associated with the relevant financing application.

---

# 5. Loan Application

## US-008 – Select Finance Institutions

### AC-010 – Display Available Finance Institutions

**Given** a valid financing application exists,

**When** the Finance Advisor proceeds to finance institution selection,

**Then** the system shall display the available partnered finance institutions.

---

### AC-011 – Select Finance Institution

**Given** available finance institutions are displayed,

**When** the Finance Advisor selects one or more institutions,

**Then** the system shall store the selected institutions for the financing application.

---

### AC-012 – Prevent Submission Without Institution

**Given** no finance institution has been selected,

**When** the Finance Advisor attempts to proceed with the financing application,

**Then** the system shall require at least one finance institution to be selected.

---

## US-011 – Submit Loan Application

### AC-013 – Review Before Submission

**Given** the customer, vehicle, and financing information has been entered,

**When** the Finance Advisor chooses to submit the application,

**Then** the system shall allow the advisor to review the application information before submission.

---

### AC-014 – Submit Completed Application

**Given** all mandatory information has been completed and validated,

**When** the Finance Advisor confirms the application,

**Then** the system shall initiate the application submission process.

---

### AC-015 – Prevent Incomplete Submission

**Given** mandatory information is missing or invalid,

**When** the Finance Advisor attempts to submit the application,

**Then** the system shall prevent the submission and identify the information that needs to be completed or corrected.

---

## US-012 – Receive Financing Offers

### AC-016 – Receive Finance Institution Response

**Given** a financing application has been submitted to a selected finance institution,

**When** the finance institution provides a response,

**Then** the system shall receive and associate the response with the relevant financing application.

---

### AC-017 – Display Financing Offer

**Given** a finance institution has returned a financing offer,

**When** the Finance Advisor opens the application,

**Then** the system shall display the available financing offer information.

---

### AC-018 – Support Multiple Responses

**Given** an application has been submitted to multiple finance institutions,

**When** responses are received,

**Then** the system shall display the responses separately for each finance institution.

---

# 6. OCR Processing

## US-014 – Extract Customer Data Using OCR

### AC-019 – Upload Document for OCR

**Given** the Finance Advisor has a customer document,

**When** the advisor uploads the document,

**Then** the system shall make the document available for OCR processing.

---

### AC-020 – Extract Customer Information

**Given** a supported customer document has been uploaded,

**When** OCR processing is completed,

**Then** the system shall extract the relevant customer information from the document.

---

### AC-021 – Populate Customer Information

**Given** customer information has been successfully extracted,

**When** OCR processing is completed,

**Then** the extracted information shall be made available in the relevant customer fields.

---

## US-015 – Validate OCR Results

### AC-022 – Display Extracted Information

**Given** OCR processing has been completed,

**When** the Finance Advisor opens the extracted information,

**Then** the system shall display the extracted informations for a review.

---

### AC-023 – Edit OCR Results

**Given** OCR-extracted information contains an incorrect or incomplete value,

**When** the Finance Advisor reviews the information,

**Then** the advisor shall be able to edit the extracted informations.

---

### AC-024 – Confirm OCR Information

**Given** the Finance Advisor has reviewed and corrected the OCR results where necessary,

**When** the advisor confirms the extracted information,

**Then** the validated information shall be available for the financing application.

---

# 7. RPA Automation

## US-019 – Trigger RPA Process

### AC-025 – Trigger RPA After Confirmation

**Given** the financing application has been completed and reviewed,

**When** the Finance Advisor confirms the application for submission,

**Then** the RPA process shall be initiated.

---

### AC-026 – Process Selected Finance Institutions

**Given** one or more finance institutions have been selected,

**When** the RPA process starts,

**Then** the RPA process shall process the application for the selected finance institutions.

---

### AC-027 – Transfer Application Information

**Given** the RPA process has been initiated,

**When** the RPA accesses finance institutions portal,

**Then** the relevant validated application information shall be transferred to the corresponding fields.

---

## US-020 – Complete Customer SMS Verification

### AC-028 – Pause for SMS Verification

**Given** the RPA process reaches a customer SMS verification step,

**When** the finance institution requests the verification code,

**Then** the RPA process shall wait for the verification step to be completed.

---

### AC-029 – Enter Customer Verification Code

**Given** the customer has received the SMS verification code,

**When** the Finance Advisor enters the code,

**Then** the system shall submit the verification code to the relevant finance institution portal.

---

### AC-030 – Continue RPA After Verification

**Given** the SMS verification code has been accepted,

**When** verification is completed successfully,

**Then** the RPA process shall continue with the financing application process.

---

# 8. Application Tracking

## US-023 – Track Application Status

### AC-031 – Display Application Status

**Given** a financing application exists,

**When** the Finance Advisor opens the application,

**Then** the system shall display the current application status.

---

### AC-032 – Update Application Status

**Given** a finance institution provides an updated application result,

**When** the response is received,

**Then** the system shall update the corresponding application status.

---

### AC-033 – View Status Across Applications

**Given** multiple financing applications exist,

**When** the Finance Advisor accesses the application tracking view,

**Then** the system shall display the relevant applications and their current statuses.

---

# 9. Reporting

## US-026 – Monitor Financing Applications and Performance

### AC-034 – Display Financing Applications

**Given** financing applications exist in the system,

**When** the Finance Advisor opens the application dashboard,

**Then** the system shall display the available financing applications and their current statuses.

---

### AC-035 – Filter Applications

**Given** multiple financing applications are displayed,

**When** the Finance Advisor applies an available filter,

**Then** the system shall display only the applications matching the selected criteria.

---

### AC-036 – Filter by Finance Institution

**Given** applications have been submitted to different finance institutions,

**When** the Finance Advisor selects a finance institution filter,

**Then** the system shall display applications associated with the selected institution.

---

### AC-037 – Filter by Date

**Given** financing applications exist for different dates,

**When** the Finance Advisor selects a date or date range,

**Then** the system shall display applications matching the selected period.

---

### AC-038 – Monitor Operational Performance

**Given** financing application and processing data is available,

**When** the Finance Advisor accesses the performance view,

**Then** the system shall display the relevant operational performance information available to the user.

---

# 10. Acceptance Criteria Summary

| Story | Acceptance Criteria |
| ------ | ------------------- |
| US-001 | AC-001 – AC-003 |
| US-003 | AC-004 – AC-006 |
| US-005 | AC-007 – AC-009 |
| US-008 | AC-010 – AC-012 |
| US-011 | AC-013 – AC-015 |
| US-012 | AC-016 – AC-018 |
| US-014 | AC-019 – AC-021 |
| US-015 | AC-022 – AC-024 |
| US-019 | AC-025 – AC-027 |
| US-020 | AC-028 – AC-030 |
| US-023 | AC-031 – AC-033 |
| US-026 | AC-034 – AC-038 |
