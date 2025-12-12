
---

# Evaluizer Demo Flow

**Making evaluation concrete, inspectable, and maintainable**

## Purpose of the demo (internal)

* Reduce fear around “long, unstructured evaluation”
* Show that evaluation is **operational**, not theoretical
* Demonstrate continuity **after** the engagement ends
* Reinforce that this is *not* model magic, but disciplined process

This demo is **not technical**.
It is about *how decisions are supported*.

---

## When to use this demo

* After a positive intro call
* After the SME Evaluation Workshop
* Before finalizing scope or contract
* With stakeholders worried about:

  * maintenance
  * regression
  * “what happens when you leave”

---

## Demo duration

* **10–15 minutes**
* Live screen share *or* narrated screenshots
* No deep dives into code or models

---

## Demo structure (step-by-step)

---

## Step 1 — Start with the evaluation dataset (2–3 minutes)

**What you show**

The Evaluizer interface with:

* a list of evaluation questions
* grouped by risk tier (e.g. high-risk, informational, refusal cases)

**What you say**

> Before we look at any answers, we start with the evaluation set.
>
> These are questions defined or validated by your SMEs — not generic prompts.
>
> This dataset represents *what matters* in your domain, including edge cases and questions the system should refuse to answer.

**Key message**

* Evaluation starts with **domain judgment**, not model output.

---

## Step 2 — Inspect answers side-by-side (3 minutes)

**What you show**

* One evaluation question
* Multiple model outputs (or multiple prompt versions)
* Source references (if available)

**What you say**

> Here we can inspect answers side-by-side against the same question.
>
> The goal is not to ask “which answer sounds best”, but:
>
> * Is it complete?
> * Is it grounded in the right documents?
> * Does it introduce information that should not be there?
> * Should it have refused instead?

**Key message**

* Answers are **inspectable**, not opaque.

---

## Step 3 — Manual annotation with SMEs (2–3 minutes)

**What you show**

* Annotation fields (pass / fail, error type, comments)

**What you say**

> SMEs can annotate answers directly:
>
> * mark failure modes (e.g. hallucination, omission)
> * flag unacceptable behavior
> * add short comments explaining why
>
> This turns expert judgment into a reusable evaluation artifact.

**Key message**

* SME knowledge is **captured**, not lost in meetings.

---

## Step 4 — Automated evaluation & scoring (2–3 minutes)

**What you show**

* Aggregate scores
* Pass/fail counts
* Error distribution by type

**What you say**

> Once acceptance criteria are defined, Evaluizer can run automated checks:
>
> * deterministic rules
> * LLM-based judges
> * or combinations of both
>
> These scores don’t replace human judgment — they make changes *visible* and *comparable* over time.

**Key message**

* Evaluation is **repeatable**, not subjective every time.

---

## Step 5 — Comparing changes over time (2–3 minutes)

**What you show**

* Comparison between:

  * two prompt versions
  * or before/after a data change

**What you say**

> This is where evaluation really pays off.
>
> When something changes — a prompt, a document set, a model — you can immediately see:
>
> * what improved
> * what regressed
> * whether risk increased or decreased
>
> This prevents silent degradation.

**Key message**

* No more “it seemed better yesterday”.

---

## Step 6 — Handover & continuity (2 minutes)

**What you show**

* Clean project structure
* Saved evaluation sets
* Clear naming/versioning

**What you say**

> At the end of the engagement, this setup is handed over:
>
> * your evaluation dataset
> * your acceptance criteria
> * your evaluation workflow
>
> Internal teams can continue running evaluations without my involvement.
>
> This avoids vendor lock-in and reduces long-term risk.

**Key message**

* You are **not dependent** on the consultant.

---

## What you explicitly do NOT demo

* Model internals
* Embeddings
* Vector databases
* Prompt “cleverness”
* Optimization tricks

If asked, you say:

> Those choices only matter *after* evaluation criteria are clear.

---

## Typical stakeholder reactions (and how to respond)

### “This looks slower than just building something”

> It’s slower than a demo — and much faster than recovering trust after a failed deployment.

### “Can our team use this later?”

> Yes. The evaluation setup is explicitly designed for internal continuation.

### “Does this guarantee correctness?”

> No system can guarantee correctness. This makes risks explicit and measurable.

---

## Positioning sentence (use verbatim)

> Evaluizer turns evaluation from a vague promise into a concrete, inspectable workflow that aligns AI behavior with domain risk.

---

## Consultant’s internal note

This demo:

* reassures risk-averse stakeholders
* filters out “move fast” clients
* reinforces your evaluation-first positioning
* justifies your fee without talking about price

---
