
---

# 15-Minute Intro Call Script

**Evaluation-First Knowledge System Assessment & Prototype**

## Goal of the call (internal)

* Qualify fast: **is this a good fit** and **is there a real problem**
* Align expectations: **not a chatbot demo**, **not production**
* Secure next step: either **SME workshop** or **polite no**

## Tone

Calm, structured, senior. No hype.

---

## 0:00–0:45 — Opening

**You say:**

> Thanks for taking the time. To make this useful, I suggest a short structure:
> I’ll briefly explain how I work (2 minutes), then I’ll ask a few questions about your context (8–9 minutes), and we’ll close with a clear next step (2–3 minutes). Does that work?

*(If they say yes, proceed. If they go off-track early, gently return to the structure.)*

---

## 0:45–2:30 — What you do (your positioning, short)

**You say:**

> I help organizations design **AI-assisted knowledge systems that can be meaningfully evaluated and governed before deployment**.
> Most GenAI efforts fail because success criteria and failure modes are not defined in a domain-specific way.
> My approach is evaluation-first: we co-design acceptance criteria and an evaluation set with SMEs, then build a small instrumented prototype to test feasibility and risk.
> The deliverable is a clear decision: proceed, iterate, or stop — with evidence.

**Optional (if they ask “why you?”):**

> My background is in data science, governance/decision-making, and cybersecurity in regulated environments — so I’m conservative by design.

---

## 2:30–11:30 — Qualification questions (pick 6–8, don’t rush)

### A) Use case & decisions (must-have)

1. **Decision:**

> What decision(s) would this system support? What changes if the answer is good?

2. **Users:**

> Who would use it day-to-day, and who would be accountable for outcomes?

3. **Current workflow pain:**

> How do people solve this today — searching, asking colleagues, reinventing, manual review?

### B) Risk & failure tolerance (must-have)

4. **Cost of being wrong:**

> What happens if the system gives a confident but incorrect answer?

5. **Refusal design:**

> Are there question types where the system should *never* answer and must refuse?

6. **Auditability / explainability:**

> Do you need citations, traceability to documents, or an audit trail?

### C) Data reality check (must-have)

7. **Data types:**

> What documents are we talking about (policies, procedures, reports, tickets, emails, contracts, etc.)?

8. **Access constraints:**

> Any restrictions around where the data can be processed (on-prem only, CH/EU cloud only, strict access controls)?

### D) Organizational readiness (nice-to-have)

9. **SME availability:**

> Who are the 2–4 SMEs who could join a structured evaluation workshop?

10. **Success criteria:**

> If we did this well, what would you want to see at the end of 6–8 weeks?

**Your rule:** If they can’t name SMEs or a decision owner, this is not ready.

---

## 11:30–13:30 — Reflect back & frame the fit

**You say (summarize in 20–30 seconds):**

> Let me reflect back what I heard:
> You want to support [DECISION] for [USERS], using [DATA], with constraints around [GOV/SEC], and the main risk is [RISK]. Is that accurate?

Then:

**If fit is good:**

> This sounds like a good fit for an evaluation-first assessment. The next step would be a structured SME workshop to define acceptance criteria, failure modes, and an initial evaluation set.

**If fit is weak:**

> Based on what you described, I’m not sure this is the right time to build anything yet. The missing piece is [SMEs / data access / decision ownership]. If you address that, we can revisit.

---

## 13:30–15:00 — Close with a concrete next step

### Option 1: Schedule the SME Evaluation Workshop (best)

**You say:**

> If you’re open to it, I suggest a 90–120 minute workshop with 2–4 SMEs and a process owner.
> Pre-work is light: 5–10 sample documents and 5–10 real questions people ask today.
> After the workshop, I can confirm scope and deliverables precisely.

### Option 2: Request a small data sample first (when access is unclear)

**You say:**

> If workshop scheduling is hard right now, we can start with a small document sample and a question list. I’ll review it and propose a workshop agenda tailored to your domain.

### Option 3: Decline politely (protect your time)

**You say:**

> I don’t want to waste your time. Without [SME availability / data access / decision owner], this will likely become a demo without evaluation rigor. If you can align those pieces, I’d be happy to pick it up again.

---

# What you do NOT say (common traps)

* Don’t promise “95% accuracy” or any number.
* Don’t say “we’ll eliminate hallucinations.”
* Don’t say “enterprise-grade” unless asked; show it via method.
* Don’t offer operations, uptime, maintenance.
* Don’t discuss tools/models early (Evaluizer, embeddings, etc.) unless they ask.

---

# If they ask about Evaluizer (30-second answer)

**You say:**

> I use an evaluation interface so SMEs can review outputs against an evaluation dataset, annotate results, and run repeatable checks over time.
> It makes the evaluation process concrete and helps internal teams continue evaluation after the engagement.

*(Stop there. Offer a demo later, not now.)*

---

# Quick red flags (end early if 2+ occur)

* “We just want a chatbot quickly”
* No SME time available
* No data access path
* No clear decision owner
* They want production deployment + support from you
* They insist on vendor-like guarantees

---

# Success criteria for this call (internal)

* ✅ Identified decision owner + SMEs
* ✅ Understood risk tolerance and refusal needs
* ✅ Confirmed data types + constraints
* ✅ Agreed next step: SME workshop (preferred) or data sample review

---
