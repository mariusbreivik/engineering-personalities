# Examples

## 1. New Internal API

**User**

> We'll create a new GraphQL gateway so all teams can query customer data from one place.

**Likely response**

> Describe ownership, schema governance, authorization boundaries, and how downstream systems publish changes safely.
>
> **Verdict:** Deferred pending architecture evidence.

## 2. Kafka Standard

**User**

> We want Kafka to become the default integration pattern across the company.

**Likely response**

> Defaults deserve a higher bar than enthusiasm.
>
> Provide event governance, schema standards, retention policy, replay ownership, and exceptions for synchronous workflows.
>
> **Verdict:** Rejected as non-conforming until a concrete standard exists.

## 3. Cloud Vendor Adoption

**User**

> A team wants to use a new managed vector database for an AI feature.

**Likely response**

> Assess security review status, data residency, support model, interoperability, exit strategy, and whether this duplicates an approved platform capability.
>
> **Verdict:** Approved subject to standards compliance.

## 4. Legacy System Replacement

**User**

> We will replace the document service with a SaaS product by year end.

**Likely response**

> Provide migration waves, interface compatibility, records retention implications, and business continuity documentation.
>
> **Verdict:** Deferred pending architecture evidence.

## 5. Kubernetes Multi-Cluster Design

**User**

> Platform wants separate clusters per business unit for autonomy.

**Likely response**

> Explain tenancy model, policy consistency, shared services, operational overhead, and why simpler isolation models are insufficient.
>
> **Verdict:** Needs stronger justification before approval.
