
---

# Proposal

**Evaluation-First Knowledge System Assessment & Prototype**

**Client:** [Organization name]
**Date:** [Date]
**Prepared by:** Fatih Ünal

---

## 1. Context & Objective

[Organization] is exploring the use of **AI-assisted knowledge systems** to support decisions related to:

* **Decision(s):** [brief description]
* **Users:** [roles / functions]
* **Primary risk:** [e.g. incorrect, incomplete, or outdated answers]

The objective of this engagement is **not to deploy a production system**, but to determine **whether such a system can be trusted in this domain**, and under which conditions.

---

## 2. Why an evaluation-first approach

Industry experience shows that most GenAI initiatives fail in practice because:

* success criteria are implicit or undefined
* evaluation does not reflect real decision risk
* failure modes are discovered too late
* there is no mechanism for ongoing assessment

This engagement is designed around a different principle:

> **If a system cannot be meaningfully evaluated in its domain context, it should not be deployed.**

---

## 3. Scope of the engagement (6–8 weeks)

### 3.1 Use-case & risk framing

* Clarify supported decisions and accountability
* Identify unacceptable vs tolerable failure modes
* Define when the system must refuse to answer

**Deliverable:**
Problem & risk framing document

---

### 3.2 Data & governance readiness

* Review document types and structure
* Assess sensitivity, access constraints, and audit requirements
* Identify data gaps and no-go signals

**Deliverable:**
Data readiness & governance memo

---

### 3.3 Joint evaluation & system design (with SMEs)

Structured working sessions with Subject Matter Experts to define:

* domain-specific success and failure criteria
* error taxonomy and refusal rules
* acceptance thresholds aligned to organizational risk
* initial evaluation dataset (SME-authored or validated)

**Deliverables:**

* Evaluation design document
* Initial evaluation dataset

---

### 3.4 Evaluation-guided prototype

Implementation of a **limited-scope, instrumented prototype** to:

* run batch evaluations against agreed criteria
* analyze failure modes and trade-offs
* support regression testing as prompts or data change

The prototype serves as a **test harness**, not a production system.

**Deliverables:**

* Instrumented prototype
* Evaluation report with failure analysis

---

### 3.5 Decision memo

A structured recommendation covering:

* feasibility against acceptance criteria
* remaining risks and constraints
* effort required to proceed
* recommendation to proceed, iterate, or stop

**Deliverable:**
Decision memo suitable for management and governance review

---

## 4. Evaluation infrastructure

As part of the engagement, an **evaluation interface and workflow** is provided based on *Evaluizer*, an open-source framework for systematic LLM evaluation.

This enables:

* transparent review of model outputs against evaluation datasets
* manual annotation by SMEs
* automated checks using deterministic functions and LLM judges
* continued evaluation after the engagement concludes

The tooling is configured for the specific use case and handed over as part of the delivery.

---

## 5. Engagement model

* Fixed scope
* Fixed duration (6–8 weeks)
* Limited number of concurrent clients
* No production deployment
* No ongoing operational responsibility

Work is conducted independently using client-provided data and environments.

---

## 6. Roles & expectations

**Client provides:**

* access to representative documents
* availability of 2–4 SMEs for evaluation workshops
* a decision owner for scoping and sign-off

**Consultant provides:**

* evaluation-first methodology
* facilitation of SME workshops
* prototype and evaluation artifacts
* independent recommendation

---

## 7. Commercials

**Fee:** CHF [XX’000] (fixed)
**Payment terms:** [e.g. 50% start / 50% end]
**Start date:** [date]

No licenses or recurring fees.

---

## 8. Independence & IP

All work is conducted independently and uses only client-provided or publicly available materials.
No confidential or proprietary information of third parties is reused or derived.

---

## 9. Next step

Upon confirmation, the engagement starts with scheduling the **SME Evaluation Workshop**, followed by document review and detailed planning.

---

### Consultant note (internal)

This proposal is intentionally conservative.
If a client pushes for speed, production, or guarantees → **decline or re-scope**.

---

## What we’ve achieved so far

At this point you have:

* a **clear service**
* a **repeatable sales call**
* a **proposal that matches the call**
* consistent language across all artifacts

This is already a complete consulting “machine”.

---

## Next (final artifact in this set)

👉 **`05_tools_evaluizer/evaluizer_demo_flow.md`**
A short, non-technical demo flow you can:

* show in follow-up calls
* include screenshots from later
* use to reduce fear around “maintenance after you leave”

When you’re ready, say:

> “Proceed with the Evaluizer demo flow.”

We’ll keep it tight and usable.
