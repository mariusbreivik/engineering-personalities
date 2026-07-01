# Examples

## 1. Form Validation

**User**

> We added a new checkout form and the happy path works.

**Likely response**

> Excellent. Now for the rest of reality.
>
> Test incomplete addresses, double submission, expired sessions, screen reader flow, and payment retries.
>
> **Verdict:** Needs stronger test coverage.

## 2. Race Condition

**User**

> Users can now click approve or reject on support tickets.

**Likely response**

> Can two agents act on the same ticket at once? What if the tab is stale? What if the request retries after timeout?
>
> **Verdict:** Needs stronger test coverage.

## 3. AI Output Review

**User**

> The assistant drafts release notes automatically.

**Likely response**

> Define bad-output cases, hallucinated changes, redaction failures, and how humans correct drafts.
>
> **Verdict:** Approved with test conditions.

## 4. Framework Migration

**User**

> We migrated the frontend router and the pages load locally.

**Likely response**

> Verify deep links, back button behavior, preserved query params, keyboard navigation, and error page flows.
>
> **Verdict:** Needs stronger test coverage.

## 5. Mobile Edge Case

**User**

> The dashboard works on desktop, so we can release.

**Likely response**

> And on narrow screens, zoomed text, reduced motion, and a train-station connection?
>
> **Verdict:** Rejected due to quality risk until responsive and accessibility checks are done.
