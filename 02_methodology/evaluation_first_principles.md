
---

# Evaluation-First Principles

## How trustworthy AI-assisted knowledge systems are designed

---

## Principle 1 — Evaluation precedes optimization

AI-assisted knowledge systems must be evaluated **before** they are optimized.

In practice, many systems are tuned for fluency or apparent accuracy without a clear definition of what constitutes acceptable behavior. This leads to systems that perform well in demonstrations but fail in real decision contexts.

Experienced practitioners consistently emphasize that **optimization without prior evaluation is meaningless**, because there is no stable reference for improvement [1].

Evaluation therefore acts as the **specification layer** of the system, not a validation step applied at the end.

---

## Principle 2 — Evaluation must be domain-specific

Generic benchmarks and abstract accuracy scores are insufficient for real-world use.

What matters is whether system behavior is acceptable **within a specific domain**, under real constraints, for concrete decisions. Acceptability cannot be inferred from model performance alone.

Applied AI research and industry practice show that **task- and domain-specific evaluation** is required to surface meaningful failure modes and prevent silent errors [2][3].

---

## Principle 3 — Subject Matter Experts define acceptability

Only Subject Matter Experts (SMEs) can define:

* what constitutes an acceptable answer
* which errors are tolerable
* which failures are unacceptable regardless of frequency

SMEs are not asked to evaluate model internals.
They define **decision risk and acceptance criteria**.

Human-in-the-loop and expert-grounded evaluation approaches are widely recognized as necessary in high-stakes and regulated settings, where correctness is contextual rather than purely statistical [3][4].

---

## Principle 4 — Refusal is a designed behavior, not a failure

In many domains, the safest answer is **no answer**.

Systems must be explicitly designed to:

* refuse questions outside their scope
* abstain when confidence is insufficient
* signal uncertainty instead of hallucinating

Refusal behavior is a **risk control mechanism**, not a deficiency.
Leading AI labs emphasize that evaluation must include when and how systems should *not* respond [5].

---

## Principle 5 — Evaluation artifacts are first-class system components

Evaluation artifacts include:

* acceptance criteria
* evaluation datasets
* failure taxonomies
* annotated system behaviors

These artifacts are not temporary scaffolding. They are reusable system components that:

* support governance and audit
* enable regression detection
* retain value even if deployment is deferred or canceled

For this reason, evaluation artifacts are treated as **deliverables**, not byproducts.

---

## Principle 6 — Decisions are evidence-based, not aspirational

The purpose of evaluation is not to justify deployment.

The outcome of an evaluation-first process is a structured decision to:

> **Proceed · Iterate · Stop**

All three outcomes are valid.
Stopping based on evidence is considered a successful outcome.

This principle aligns with emerging best practices in AI governance, which emphasize decision traceability over optimistic experimentation [1][2].

---

## Summary

An evaluation-first approach shifts AI system design from:

* model-centric thinking
* demo-driven validation
* post-hoc risk discovery

to:

* domain-anchored evaluation
* explicit failure design
* evidence-based deployment decisions

This discipline is what separates AI systems that merely impress from systems that can be trusted.

---

## References

[1] Hamel Husain — *Evals Before Optimization*
[https://hamel.dev/blog/posts/evals-faq/](https://hamel.dev/blog/posts/evals-faq/)

[2] Anthropic — *A Statistical Approach to Model Evaluations*
[https://www.anthropic.com/research/statistical-approach-to-model-evals](https://www.anthropic.com/research/statistical-approach-to-model-evals)

[3] Eugene Yan — *Productizing Machine Learning* / *ML System Failure Modes*
[https://eugeneyan.com/writing/](https://eugeneyan.com/writing/)

[4] Stanford Human-Centered AI — Evaluation in High-Stakes Domains
[https://hai.stanford.edu/research](https://hai.stanford.edu/research)

[5] OpenAI — Evaluation & System Behavior Guidance
[https://platform.openai.com/docs/guides/evals](https://platform.openai.com/docs/guides/evals)

---
