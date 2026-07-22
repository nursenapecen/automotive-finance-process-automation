# Business Rules

## Document Overview

This document defines the business rules governing the Automotive Finance Process Automation solution.

These rules describe business policies, validations, and operational constraints independent of system implementation.

## Rule Categories

| Prefix  | Category     |
| ------- | ------------ |
| BR-CUS  | Customer     |
| BR-VEH  | Vehicle      |
| BR-LOAN | Loan         |
| BR-CMP  | Campaign     |
| BR-FIN  | Finance Institution Rules   |
| BR-OCR  | OCR          |
| BR-RPA  | RPA          |
| BR-NOT  | Notification |
| BR-SEC  | Security     |
| BR-REP  | Reporting   |
| BR-VAL  | Validation   |
| BR-EXC  | Exception Rules  |


## 1. Customer Rules

BR-CUS-001

Customer Identity Number shall be mandatory.

BR-CUS-002

Customer mobile phone number shall be mandatory.

BR-CUS-003

Each financing application shall belong to one customer only.

BR-CUS-004

Customer identity information shall be validated before application submission.

BR-CUS-005

Customer address information shall be completed before submission.

BR-CUS-006

Incomplete customer information shall prevent loan application submission.


## 2. Vehicle Rules

BR-VEH-001

Each financing application shall contain exactly one vehicle.

BR-VEH-002

Vehicle information shall match ERP records.

BR-VEH-003

Vehicle invoice amount shall be greater than zero.

BR-VEH-004

Vehicle type shall be either New or Used.

BR-VEH-005

Tax exemption shall only be applicable when explicitly selected.


## 3. Loan Application Rules

BR-LOAN-001

At least one finance institution shall be selected.

BR-LOAN-002

One application may be submitted to multiple finance institutions.

BR-LOAN-003

Loan amount shall not exceed vehicle invoice amount.

BR-LOAN-004

Loan maturity shall comply with finance institution policies.

BR-LOAN-005

Application status shall be updated after every finance institution response.

BR-LOAN-006

Each application shall have a unique Application ID.

BR-LOAN-007

Application cannot be submitted twice to the same finance institution.


## 4. Campaign Rules

BR-CMP-001

Campaign selection shall be performed before loan submission.

BR-CMP-002

Only active campaigns shall be displayed.

BR-CMP-003

Campaign eligibility shall depend on selected vehicle and loan type.

BR-CMP-004

Campaign selection shall be editable before submission.


## 5. Finance Institution Rules

BR-FIN-001

Users may select multiple finance institutions.

BR-FIN-002

Each finance institution shall receive the same validated customer information.

BR-FIN-003

Responses from finance institutions shall be stored separately.

BR-FIN-004

Finance institution responses shall not overwrite previous responses.


## 6. OCR Rules

BR-OCR-001

OCR shall process uploaded identity documents.

BR-OCR-002

OCR extracted values shall remain editable.

BR-OCR-003

Users shall verify OCR results before submission.

BR-OCR-004

Unreadable documents shall require manual data entry.

BR-OCR-005

Original uploaded documents shall be stored.


## 7. RPA Rules

BR-RPA-001

RPA shall start only after advisor confirmation.

BR-RPA-002

RPA shall stop when OTP verification is required.

BR-RPA-003

OTP shall be entered manually by the advisor.

BR-RPA-004

RPA shall continue after successful OTP verification.

BR-RPA-005

Failed submissions shall be logged.

BR-RPA-006

RPA shall retry failed submissions according to retry policy.


## 8. Notification Rules

BR-NOT-001

Customers shall receive notifications only after application submission.

BR-NOT-002

Finance advisors shall receive notifications for rejected applications.

BR-NOT-003

Missing documents shall generate notifications.

BR-NOT-004

Application completion shall trigger confirmation notification.


## 9. Security Rules

BR-SEC-001

Only authorized users shall access financing applications.

BR-SEC-002

Sensitive customer information shall be protected.

BR-SEC-003

Every user action shall be logged.

BR-SEC-004

Deleted applications shall remain in audit history.


## 10. Reporting Rules

BR-REP-001

Applications shall be searchable by customer.

BR-REP-002

Applications shall be searchable by finance institution.

BR-REP-003

Applications shall be searchable by branch.

BR-REP-004

Application history shall be retained.


## 11. Validation Rules

BR-VAL-001

Mandatory fields shall be completed before submission.

BR-VAL-002

Loan amount shall be numeric.

BR-VAL-003

Identity Number shall contain exactly 11 digits.

BR-VAL-004

Phone number shall follow national format.

BR-VAL-005

Customer age shall comply with finance institution requirements.


## 12. Exception Rules

BR-EXC-001

If OCR fails, manual entry shall be allowed.

BR-EXC-002

If a finance institution portal is unavailable, the application shall remain pending.

BR-EXC-003

If OTP expires, the advisor shall request a new OTP.

BR-EXC-004

If mandatory documents are missing, submission shall not proceed.

