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

| Test Case ID | Scenario | Steps | Expected Result | Actual Result | Pass/Fail | Notes |
|-------------|---------|-------|----------------|---------------|-----------|-------|
| TC-001 | Full Payment Match | 1. Upload billing file <br> 2. Upload payment file <br> 3. Run reconciliation | Matched invoices closed, no exceptions | | | |
| TC-002-US001 | Partial Payment | 1. Upload partial payment file <br> 2. Run reconciliation | Exception flagged, invoice not closed | | | |
