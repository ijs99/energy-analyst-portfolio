| Test Case ID | Scenario | Steps | Expected Result | Actual Result | Pass/Fail | Notes |
|-------------|---------|-------|----------------|---------------|-----------|-------|
| TC-001 | Full Payment Match | 1. Upload billing file <br> 2. Upload payment file <br> 3. Run reconciliation | Matched invoices closed, no exceptions | | | |
| TC-002-US001 | Partial Payment | 1. Upload partial payment file <br> 2. Run reconciliation | Exception flagged, invoice not closed | | | |
