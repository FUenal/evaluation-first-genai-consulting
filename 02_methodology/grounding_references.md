# Grounding References
**Selective external grounding for evaluation-first claims**

This document maps **core claims** of the evaluation-first offering to **external practitioner and institutional sources**.  
References are used only where a senior stakeholder would reasonably challenge a claim as opinion.

The goal is credibility, not exhaustiveness.

---

## Claim 1  
### Most GenAI initiatives fail to translate from pilots to measurable business impact

**Why grounding is needed**  
Senior stakeholders will challenge “most fail” unless it is tied to credible institutions.

**Primary sources (institutional)**
- MIT NANDA / Project NANDA report (“The GenAI Divide: State of AI in Business 2025”) reporting that *95% of organizations are getting zero return* and highlighting that outcomes are driven by approach rather than model quality.  
- Secondary coverage (use only when the PDF is too dense for stakeholders): Fortune / Tom’s Hardware summaries referencing the report.

**Usage guidance**
- Phrase as “recent MIT NANDA / Project NANDA reporting suggests…” rather than “MIT proved”.
- Do not over-index on the number. Use it to open the door, then pivot to *why* (evaluation + integration + governance).

**Where to integrate**
- `03_sales_enablement/why_95_percent_fail_onepager.md` (primary)
- Optional: appendix note in `02_methodology/evaluation_first_principles.md`

---

## Claim 2  
### “Model quality” is not the bottleneck — evaluation and real-world constraints are

**Why grounding is needed**  
This is your differentiator: “evaluation-first” must not sound like a personal philosophy.

**Primary sources (big-company + platform)**
- OpenAI docs: evaluation best practices and guidance that generative AI is variable and traditional testing is insufficient; evals are needed to test systems in production-like conditions.  
- Anthropic research: “A statistical approach to model evaluations” stresses evaluation rigor, measurement uncertainty, and experimental design principles.

**Usage guidance**
- Use OpenAI/Anthropic as *credibility anchors* for “evals are required,” not as “endorsements” of your service.
- Keep this section very short in client-facing docs.

**Where to integrate**
- `03_sales_enablement/why_95_percent_fail_onepager.md`
- `02_methodology/evaluation_first_principles.md` (core grounding)

---

## Claim 3  
### Evaluation must be domain-specific and SME-defined

**Why grounding is needed**  
Tool-vendors and engineers often claim generic benchmarks and automated evals are enough.

**Primary sources (Ivy-league / domain eval)**
- Stanford HAI (medical/health contexts): emphasizes holistic, real-world, expert-grounded evaluation approaches for LLMs in specialized domains.

**Usage guidance**
- Emphasize SMEs define **acceptability + failure modes**, not model internals.
- Phrase as “domain experts anchor evaluation to real task demands.”

**Where to integrate**
- `02_methodology/evaluation_first_principles.md`
- Brief rationale line in `02_methodology/sme_workshop_agenda.md`

---

## Claim 4  
### Refusal / abstention is a required safety & governance control (not a failure)

**Why grounding is needed (light)**  
Some stakeholders believe partial answers are better than refusals.

**Primary sources**
- OpenAI guidance around evals + system behavior (use lightly; frame refusal as part of “specifying behavior before deployment,” not as moral philosophy).

**Usage guidance**
- Keep this to one paragraph + one reference.
- Treat refusal as a risk control: “must refuse when criteria aren’t met.”

**Where to integrate**
- `02_methodology/failure_taxonomy_reference.md`

---

## Claim 5  
### Evaluation artifacts retain value even if the system is not deployed

**Grounding status**
❌ No external grounding required.

**Rationale**
Governance and audit stakeholders already understand why decision frameworks and evaluation artifacts remain reusable.

---

## Claim 6  
### Evaluation-first reduces long-term risk and rework

**Grounding status**
⚠️ Avoid quantitative ROI claims until you have your own case studies.

**Rationale**
Without your own evidence, external ROI claims are easy to attack and create false expectations.

**Where to integrate**
Verbal only (for now). Optionally in future, after 1–2 engagements with permissioned case studies.

---

## Approved reference shortlist (do not expand casually)

**Institutional**
[1] MIT / Project NANDA — The GenAI Divide: State of AI in Business 2025
https://mlq.ai/media/quarterly_decks/v0.1_State_of_AI_in_Business_2025_Report.pdf
[5] Stanford Human-Centered AI — Evaluation in High-Stakes Domains
https://hai.stanford.edu/research

**Big-company / platform**
References
[2] Hamel Husain — Evals Before Optimization
https://hamel.dev/blog/posts/evals-faq/
[3] Eugene Yan — Productizing Machine Learning / ML System Failure Modes
https://eugeneyan.com/writing/
[4] Anthropic — A Statistical Approach to Model Evaluations
https://www.anthropic.com/research/statistical-approach-to-model-evals
[6] Jason Snyder (Forbes) — MIT Finds 95% of GenAI Pilots Fail Because Companies Avoid Friction
https://www.forbes.com/sites/jasonsnyder/2025/08/26/mit-finds-95-of-genai-pilots-fail-because-companies-avoid-friction/
[7] Shreya Shankar — AI Engineering: The Missing Discipline
https://www.sh-reya.com/blog/ai-engineering-short/

