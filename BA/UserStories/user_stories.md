# US-001: System automatically reconciles full payments
**Epic:** EPIC-001

## Story
As a Billing Officer, I want the system to automatically reconcile payments to invoices so that I can focus only on exceptions.

## Acceptance criteria:
- Given daily billing and payments files, when the reconciliation runs, then matched invoices are closed and exceptions are listed.
- Match rate >= 95% on day 1 for standard invoices.

---

# US-002: Flag Partial Payments
**Epic:** EPIC-001

## Story
As a Billing Officer, I want the system to flag partial payments automatically, So that exception are reviewed quickly.

## Acceptance criteria:
- Given a customer invoice is partially paid, when reconciliation runs, then the invoice is flagged as an exception.
- The flagged invoice appears in the exception report for the Billing Officer.
- Notifications are generated for invoices flagged as exceptions.

---

# US-003: Notify Customer Care of Failed Reconciliations
**Epic:** EPIC-001

## Story
As a Customer Care agent, I want notifications of failed reconciliations, so that I can proactively contact affected customers.

## Acceptance Criteria:
= Given a reconciliation fails for any invoice, when the system processes daily reconciliations, then Customer Care receives a notification with invoice details.
- The notification includes customer name, invoice number, amount, and failure reason.
- Only invoices with unresolved exceptions are notified.

---

# US-004: Daily Reconciliation Summary for Finance
**Epic:** EPIC-001

## Story
As a Finance Manager, I want a daily reconciliation summary report, so that I can track billing accuracy.

## Acceptance Criteria
- Given the daily reconciliation completes, when the report is generated, then it shows total invoices processed, matched invoices, exceptions, and match rate.
- The report is delivered to Finance manger by 8 AM daily.
- Match rate >= 95% is highlighted in green; below 95% is highlighted in red.

---

# US-XXX:
**Epic:** EPIC-XXX

## Story
As a (actor), I want (action), so that (goal)

## Acceptance Criteria
- todo.
