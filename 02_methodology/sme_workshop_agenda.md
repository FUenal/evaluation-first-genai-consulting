
---

# 1️⃣ SME Evaluation Workshop Agenda

**“From domain knowledge to evaluable system design”**

### Purpose (how you explain it to clients)

> This workshop translates domain expertise into concrete evaluation criteria, so that an AI-assisted knowledge system can be assessed meaningfully before deployment.

You are not “brainstorming prompts”.
You are **formalizing judgment**.

---

## Workshop at a glance

* **Duration:** 90–120 minutes
* **Participants:**

  * 2–4 Subject Matter Experts
  * 1 process owner / decision-maker
  * (Optional) compliance / risk representative
* **Format:** Structured, facilitated session
* **Output:** Evaluation design inputs, not technical implementation

---

## Pre-work (asynchronous, very light)

You request **before the workshop**:

* 5–10 representative documents
* 5–10 example questions people *already ask*
* A short description of decisions these answers inform

This filters unserious engagements early.

---

## Workshop Agenda (Detailed)

---

### 0. Context setting (10 minutes)

**Goal:** Align expectations and psychological safety

You explain:

* This is *not* about building a chatbot
* Wrong answers matter more than impressive answers
* Refusal to answer is a valid outcome
* Evaluation comes before optimization

Key sentence you say out loud:

> “If we can’t define what ‘good’ looks like, we shouldn’t automate it.”

---

### 1. Decision & risk mapping (20–25 minutes)

**Goal:** Anchor evaluation in real consequences

You facilitate answers to:

* What decisions would this system support?
* Who relies on these answers?
* What happens if the answer is wrong?
* What happens if the answer is incomplete?
* What happens if the answer sounds confident but is outdated?

You explicitly surface:

* *high-risk vs low-risk questions*
* *where human judgment must remain*

**Output:**

* Decision categories
* Risk tiers (e.g. unacceptable / tolerable / informational)

---

### 2. Failure mode identification (20–25 minutes)

**Goal:** Make errors explicit and discussable

You guide SMEs through a **failure taxonomy**, such as:

* hallucination (fabricated facts)
* omission (missing critical constraints)
* ambiguity (multiple interpretations)
* outdated information
* misapplied policy
* overconfident tone
* inappropriate refusal

You ask:

* Which of these are unacceptable?
* Which are tolerable?
* Which should trigger refusal?

**Output:**

* Domain-specific error taxonomy
* Initial refusal rules

This is where trust is built.

---

### 3. Defining “acceptable answers” (20–25 minutes)

**Goal:** Move beyond vague notions of correctness

You work with SMEs to define:

* what *must* be present in a good answer
* what *must never* be present
* when uncertainty should be expressed
* when sources must be cited or constrained

You avoid accuracy percentages.
You talk about **answer properties**.

**Output:**

* Acceptance criteria
* Qualitative scoring dimensions

---

### 4. Evaluation dataset design (20 minutes)

**Goal:** Turn expertise into test cases

Together, you define:

* representative questions per risk tier
* edge cases and “trap questions”
* examples that should trigger refusal
* examples where partial answers are acceptable

You explicitly state:

> “This is not training data. This is test data.”

**Output:**

* Initial evaluation question set
* SME-validated expected behaviors

---

### 5. Handover & next steps (10 minutes)

**Goal:** Close cleanly and confidently

You explain:

* how these outputs feed into the prototype
* how Evaluizer will be used to run and inspect evaluations
* what will be tested and what will not
* how results will be reviewed together

You do *not* promise performance.

---

## Workshop Deliverables (what you list in proposals)

* Decision & risk map
* Domain-specific error taxonomy
* Acceptance & refusal criteria
* SME-authored evaluation question set

This alone is worth money.

---

## Why this workshop is a sales accelerator

From a consultant’s perspective:

* it filters unserious clients
* it demonstrates rigor immediately
* it reframes GenAI as a governance problem
* it positions you as a facilitator of judgment, not a tool builder

---
