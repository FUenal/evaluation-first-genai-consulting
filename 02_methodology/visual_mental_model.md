
---

# The Evaluation-First Mental Model

## How trustworthy AI-assisted knowledge systems are decided, not assumed

---

## Core idea (one sentence)

> **Trustworthy AI systems are not built first and evaluated later — they are evaluated first, and only then allowed to exist.**

---

## The model at a glance (conceptual flow)

```
Domain & Risk Context
        ↓
SME-Defined Acceptance Criteria
        ↓
Failure Taxonomy
        ↓
Evaluation & Evidence
        ↓
Decision: Proceed · Iterate · Stop
```

Each layer constrains the next.
Skipping a layer invalidates everything downstream.

---

## Layer 1 — Domain & risk context

**Key question**

> What decision would this system support, and what is the cost of being wrong?

**What is defined**

* decision scope
* accountability
* regulatory or governance constraints
* unacceptable outcomes

**Why this matters**
Without explicit risk context, “accuracy” is meaningless.

---

## Layer 2 — SME-defined acceptance criteria

**Key question**

> What does “acceptable behavior” mean in this domain?

**What is defined**

* what a correct answer looks like
* what errors are tolerable vs unacceptable
* when the system must refuse to answer

**Who defines this**

* Subject Matter Experts (not engineers, not vendors)

**Why this matters**
Only domain experts can define decision acceptability.

---

## Layer 3 — Failure taxonomy

**Key question**

> How can this system fail in ways that matter?

**What is defined**

* hallucination
* unsupported inference
* omission
* overconfidence
* refusal failure
* misalignment with domain norms

**Why this matters**
Trust is determined by *how systems fail*, not how often they succeed.

---

## Layer 4 — Evaluation & evidence

**Key question**

> How does the system behave when tested against real decision scenarios?

**What happens**

* evaluation datasets reflect real use cases
* system outputs are inspected and annotated
* failures are classified using the taxonomy
* trade-offs and irreducible risks are surfaced

**What this produces**

* evidence, not impressions
* traceable evaluation artifacts

---

## Layer 5 — Decision

**Key question**

> Based on evidence, should this system exist?

**Possible outcomes**

* **Proceed** — risks are acceptable
* **Iterate** — risks can be reduced
* **Stop** — risks are unacceptable

All three outcomes are valid.

**Why this matters**
The goal is not deployment.
The goal is a **defensible decision**.

---

## What this model prevents

This model explicitly prevents:

* demo-driven deployments
* optimism bias (“it will get better”)
* model-centric decision-making
* late discovery of unacceptable behavior
* post-hoc governance justification

---

## What this model enables

This model enables:

* early detection of no-go scenarios
* transparent trade-off discussions
* SME authority without technical burden
* audit-ready decision trails
* trust that survives scrutiny

---

## Relationship to tooling

This model is **tool-agnostic**.

Evaluation tooling (e.g. Evaluizer) is used to operationalize:

* annotation
* aggregation
* regression tracking

Tooling does not define:

* acceptance criteria
* failure categories
* decisions

Those remain human and domain-anchored.

---

## One-line takeaway (for slides or website)

> **Evaluation defines whether an AI system is allowed to exist — not how impressive it looks.**

---
