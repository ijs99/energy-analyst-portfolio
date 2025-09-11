# UAT Tracker - Automated Bill Reconciliation
**Epic:** EPIC-001  
**Author:** Ismael Sanchez  
**Date:** 2025-09-11  

## Summary
- Total Test Cases: TBD  
- Passed: TBD  
- Failed: TBD  
- Blocked: TBD  

---


## US-001: System automatically reconciles full payments
| Test Case ID | Scenario | Steps | Expected Result | Actual Result | Pass/Fail | Notes |
|-------------|---------|-------|----------------|---------------|-----------|-------|
| TC-001-US001 | Full Payment Match | 1. Upload daily billing file<br>2. Upload daily payment file<br>3. Run reconciliation | System flags all partial payments as exceptions ||||
| TC-002-US001 | Partial Payment Present | 1. Upload billing file<br>2. Upload partial payment file<br>3. Run reconciliation | Matched invoices closed, partial payments flagged as exceptions ||||
| TC-003-US001 | No Payment | 1. Upload billing file<br>2. No payments uploaded<br>3. Run reconciliation | All invoices flagged as exception ||||
| TC-xxx-US001 | [scenario] | 1. [step1]<br>2. [step2]<br>3. [step3] | [expected result] ||||

---
## US-002: Flag partial payments
| Test Case ID | Scenario | Steps | Expected Result | Actual Result | Pass/Fail | Notes |
|--------------|---------|-------|----------------|---------------|-----------|-------|
| TC-001-US002 | Detect Partial Payments | 1. Upload billing file<br>2. Upload partial payment file<br>3. Run reconciliation | System flags all partial payments as exceptions | | | |
| TC-002-US002 | Validate Exception Details | 1. View exceptions list<br>2. Cross-check with payment amounts | Exception list matches expected partial payments | | | |

---

## US-003: Notify Customer Care on Exception
| Test Case ID | Scenario | Steps | Expected Result | Actual Result | Pass/Fail | Notes |
|--------------|---------|-------|----------------|---------------|-----------|-------|
| TC-001-US003 | Exception Notification | 1. Run reconciliation with exceptions<br>2. Trigger notification workflow | Customer Care receives notification for each exception | | | |
| TC-002-US003 | Notification Accuracy | 1. Open notification<br>2. Compare invoice & exception details | All details match system exceptions | | | |

---

## US-004: Manual Reconciliation for Unmatched Invoices
| Test Case ID | Scenario | Steps | Expected Result | Actual Result | Pass/Fail | Notes |
|--------------|---------|-------|----------------|---------------|-----------|-------|
| TC-001-US004 | Manual Match | 1. Open unmatched invoice list<br>2. Apply payment manually<br>3. Save changes | Invoice status updated to “Closed” | | | |
| TC-002-US004 | Reject Incorrect Match | 1. Attempt to match wrong payment<br>2. Save changes | System blocks invalid match | | | |

---

## US-005: Reporting and Metrics
| Test Case ID | Scenario | Steps | Expected Result | Actual Result | Pass/Fail | Notes |
|--------------|---------|-------|----------------|---------------|-----------|-------|
| TC-001-US005 | Generate Daily Reconciliation Report | 1. Run reconciliation<br>2. Export report | Report shows total invoices, matched, partial, and exceptions | | | |
| TC-002-US005 | Report Accuracy | 1. Compare report to system data | Report matches actual system results | | | |

---

