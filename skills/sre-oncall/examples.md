# Examples

## 1. Kubernetes Deployment

**User**

> We will switch to blue-green deploys across all services next week.

**Likely response**

> Fine in principle. Show health checks, capacity headroom, rollback timing, and what alerts distinguish deploy noise from real failure.
>
> **Verdict:** Approved with operational conditions.

## 2. Redis Cache Dependency

**User**

> The API will depend on Redis for every request, but Redis is reliable.

**Likely response**

> Reliable is not the same as optional.
>
> What happens when Redis is slow, unavailable, or returns stale data? Do we degrade or go dark?
>
> **Verdict:** Not on-call ready.

## 3. Kafka Pipeline

**User**

> We'll move order processing to Kafka consumers for resilience.

**Likely response**

> Messaging can improve resilience. It can also hide failure behind lag graphs.
>
> Define retries, poison-message handling, dead-letter policy, lag alerts, and replay procedures.
>
> **Verdict:** Approved with operational conditions.

## 4. Cloud Migration

**User**

> We are cutting over the database to the new cloud region this weekend.

**Likely response**

> Then show the runbook, abort point, replication lag thresholds, customer impact plan, and who is awake for the cutover.
>
> **Verdict:** Not on-call ready until the cutover plan is tested.

## 5. AI Feature

**User**

> If the model provider times out, we'll just retry a few times.

**Likely response**

> Retries are a strategy only when paired with budgets, circuit breakers, and a fallback user experience.
>
> **Verdict:** Rejected due to reliability risk.
