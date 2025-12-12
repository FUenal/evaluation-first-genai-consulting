
---

# Failure Taxonomy

## How unacceptable system behavior is identified, classified, and evaluated

---

## Purpose of this document

This document defines a **failure taxonomy** for evaluation-first AI-assisted knowledge systems.

The taxonomy serves three purposes:

1. Provide a **shared vocabulary** for SMEs, engineers, and decision owners
2. Enable **systematic evaluation** beyond generic accuracy metrics
3. Support **governance, audit, and decision traceability**

Failures are not treated as bugs to be hidden, but as **signals that determine whether deployment is acceptable**.

---

## Core principle

> A system does not fail when it is wrong.
> A system fails when it behaves **unacceptably for its domain and risk context**.

This taxonomy is therefore **domain-agnostic in structure**, but **domain-specific in application**.

---

## Failure categories (canonical)

All system failures must be classified into **exactly one primary category**.
Secondary categories may be noted, but one must dominate.

---

## 1. Hallucination

**Category:** Critical

### Definition

The system produces information that is **not supported by the provided documents** or invents facts, entities, or relationships.

### Why this matters

Hallucination erodes trust immediately and is often indistinguishable from correct answers for non-expert users.

### Examples

* Citing a regulation that does not exist
* Inventing a policy clause
* Attributing statements to documents that do not contain them

### Evaluation rule

* **Always unacceptable** in high-stakes or regulated contexts
* Requires explicit detection and mitigation

---

## 2. Unsupported inference

**Category:** Critical

### Definition

The system draws conclusions that are **not explicitly supported** by the source material, even if they sound plausible.

### Why this matters

This is more subtle than hallucination and often goes unnoticed.

### Examples

* Inferring intent or legal meaning not stated in the text
* Combining unrelated facts into a new conclusion

### Evaluation rule

* Typically unacceptable
* SMEs must decide whether bounded inference is ever permitted

---

## 3. Omission

**Category:** High

### Definition

The system provides an answer that is technically correct but **misses critical information** required for a safe or complete decision.

### Why this matters

Partial answers can be more dangerous than incorrect ones.

### Examples

* Summarizing a policy while omitting key exceptions
* Answering a procedural question without mentioning mandatory approvals

### Evaluation rule

* Often unacceptable in decision-support contexts
* Acceptability depends on domain and task

---

## 4. Overconfidence

**Category:** High

### Definition

The system presents uncertain or ambiguous information with **unwarranted confidence**.

### Why this matters

Users tend to trust confident language, even when uncertainty should be explicit.

### Examples

* Definitive answers where documents are ambiguous
* Failure to signal uncertainty or assumptions

### Evaluation rule

* Unacceptable when uncertainty materially affects decisions
* Must be paired with uncertainty signaling or refusal

---

## 5. Refusal failure

**Category:** Critical

### Definition

The system answers a question that it **should have refused** based on scope, confidence, or policy constraints.

### Why this matters

This is a design failure, not a model limitation.

### Examples

* Answering questions outside the document corpus
* Responding to requests requiring human judgment or authority

### Evaluation rule

* Always unacceptable
* Refusal behavior must be explicitly tested

---

## 6. Over-refusal

**Category:** Medium

### Definition

The system refuses to answer questions it **should be able to answer** safely and correctly.

### Why this matters

Excessive refusal degrades usability and trust.

### Examples

* Refusing clearly supported factual questions
* Overly conservative abstention

### Evaluation rule

* Acceptable during early iterations
* Must be monitored and reduced deliberately

---

## 7. Misalignment with domain norms

**Category:** Medium

### Definition

The system produces answers that are factually correct but **inappropriate in tone, framing, or interpretation** for the domain.

### Why this matters

Domain norms encode risk, responsibility, and professionalism.

### Examples

* Legal answers phrased as informal advice
* Policy interpretations framed as recommendations

### Evaluation rule

* SMEs define acceptability
* Often unacceptable in formal or regulated settings

---

## 8. Source attribution failure

**Category:** High

### Definition

The system fails to correctly reference or attribute the source material used in its answer.

### Why this matters

Traceability is essential for audit, trust, and verification.

### Examples

* Missing citations
* Incorrect document references
* Blended sources without distinction

### Evaluation rule

* Often unacceptable where auditability is required

---

## Severity mapping (guidance)

| Category                   | Typical Severity |
| -------------------------- | ---------------- |
| Hallucination              | Critical         |
| Unsupported inference      | Critical         |
| Refusal failure            | Critical         |
| Omission                   | High             |
| Overconfidence             | High             |
| Source attribution failure | High             |
| Misalignment with norms    | Medium           |
| Over-refusal               | Medium           |

Final severity classification is **domain-dependent** and decided by SMEs.

---

## How this taxonomy is used in evaluation

During evaluation:

* Each answer is annotated with:

  * failure category (if any)
  * severity
  * short SME comment
* Aggregated results reveal:

  * dominant failure modes
  * irreducible risks
  * suitability for deployment

This enables **transparent trade-off analysis**, not binary pass/fail scoring.

---

### Operationalization note

This failure taxonomy defines *what* constitutes unacceptable behavior.  
How failures are recorded, annotated, and aggregated is described separately in the evaluation methodology and tooling documentation.

The taxonomy is intentionally tool-agnostic.

---

## Governance & audit relevance

This taxonomy:

* supports explainable deployment decisions
* documents why a system was approved, constrained, or rejected
* provides evidence for internal and external audits

Failure classification is therefore a **governance artifact**, not a technical detail.

---

## Summary

A trustworthy AI-assisted knowledge system is not defined by how often it answers correctly, but by **how it fails**.

This taxonomy ensures failures are:

* visible
* classified
* discussed
* and designed against

Without it, evaluation degenerates into anecdote.

---

## Related documents

This taxonomy is used in conjunction with:

- `evaluation_first_principles.md` — conceptual foundation of evaluation-first design  
- `sme_workshop_agenda.md` — how SMEs define acceptance criteria and failure modes  
- `evaluation_design_framework.md` — how evaluation datasets and criteria are constructed  
- `evaluizer_overview.md` — tooling used to operationalize evaluation during the engagement

---