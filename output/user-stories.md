# Approved User Stories

## 1. Submit a vacation leave request

**As an** employee, **I want** to submit a vacation leave request with a start date and end date, **so that** my manager can review it.

### Acceptance criteria

- **Given** an employee has a vacation leave request with a start date and end date, **when** they submit it, **then** the internal system makes it available for manager review.
- **Given** an employee submits a request, **when** the request is awaiting review, **then** submitting it does not itself approve the leave.

**Priority:** High — core workflow capability.

**Assumptions:** None beyond the approved clarified requirement.

**Out of scope:** Date and policy validation rules; editing or withdrawing a pending request; manager assignment and overdue or unavailable manager handling.

## 2. Review and decide on a vacation leave request

**As a** manager, **I want** to review a vacation leave request and approve or reject it, **so that** the request receives a decision and the appropriate next steps can occur.

### Acceptance criteria

- **Given** a vacation leave request is awaiting review, **when** the manager approves it, **then** the internal system records the request as approved, adds the leave to the employee’s calendar, and notifies HR.
- **Given** a vacation leave request is awaiting review, **when** the manager rejects it and provides a reason, **then** the internal system records the request as rejected and notifies the employee of the reason.
- **Given** a request is rejected, **when** its outcome is processed, **then** the leave is not added to the employee’s calendar and HR is not notified of an approval.

**Priority:** High — core workflow capability.

**Assumptions:** None beyond the approved clarified requirement. The rejection notification includes the reason provided by the manager; whether a reason is mandatory remains open.

**Out of scope:** Manager review deadlines or unavailability; notification channels and content beyond the stated rejection reason; calendar target; employee notifications for approvals.

## Open questions

- What date rules apply, such as past dates, non-working days, or an end date before the start date?
- Are leave balances, overlapping requests, minimum notice, or maximum leave duration relevant?
- Is a rejection reason required, and are there requirements for its content?
- Can an employee edit or withdraw a request while it is awaiting review?
- What happens if a manager does not review a request or is unavailable?
- How are employees and HR notified, and what should those notifications contain?
- Which calendar is updated, and should the employee be notified when a request is approved?
