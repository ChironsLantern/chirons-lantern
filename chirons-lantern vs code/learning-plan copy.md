# Step-by-Step Learning Plan (36-Month Roadmap)

**Assumption**: ~15–20 hrs/week total (learning + building). Adjust as needed.

---

## Phase 0 (Weeks 1–2): Light the Forge
- Install: VS Code, Python 3.11, Git, Node.js, Docker.
- Learn terminal basics; create your first repo; push to GitHub.
- Mini-ship: *hello_cli.py* (takes a name, prints a greeting), and *hello_api.py* (FastAPI endpoint).

**Skill gates**
- Create/clone repo, branch → PR → merge.
- Run a virtual environment, install dependencies with `pip`/`uv`/`pipx`.

---

## Phase 1 (Months 1–3): Programming Foundations (Python First)
**Topics**
- Data types, control flow, functions, modules, packages.
- Collections & algorithms (lists, dicts, sets; complexity intuition).
- OOP basics; error handling; logging.
- Testing (pytest); type hints (mypy/pyright).
- Packaging and CLI apps.

**Projects**
- *Vitals Whisperer — CLI*: calculate PACU readiness scores, timers, checklists.
- *Tiny FastAPI service*: endpoints for patients, vitals, notes; SQLite/SQLModel; tests.

**Definition of Done**
- Repo with tests & README; deployed FastAPI endpoint on Render/Fly.io.

---

## Phase 2 (Months 4–6): Full‑Stack Fundamentals
**Topics**
- Databases: SQL, schemas, relationships; Postgres; ORMs.
- REST patterns; auth (JWT / session); background jobs.
- Front-end: HTML/CSS/JS; React (or Svelte) components; forms & state.
- UX basics: user stories, wireframes, usability tests (3+ nurses).

**Projects**
- *Vitals Whisperer — Web*: React + FastAPI + Postgres; login; vitals capture; checklist flows.
- *Design system seeds* in Figma: buttons, inputs, color tokens.

**Definition of Done**
- Deployed web app with auth; seed data; simple audit log; 3 user feedback sessions.

---

## Phase 3 (Months 7–12): Data & AI Foundations
**Topics**
- Data wrangling (Pandas/Polars), tidy data, plotting (matplotlib).
- Classical ML: train/test split, metrics, baselines (logistic regression, trees).
- LLM concepts: prompting, embeddings, retrieval (vector indexes), evaluation and guardrails.
- Build an evaluation harness (dataset of Q→A + ground truth).

**Projects**
- *Chiron Node — RAG*: index de-identified policies/protocols; answer PACU questions with citations.
- *Eval Harness*: track accuracy, hallucinations, and refusal rates on a test set.

**Definition of Done**
- CLI + web demo with citations; eval report; guardrails for unsafe requests.

---

## Phase 4 (Months 13–18): Privacy, Mobile, and Workflows
**Topics**
- De-identification/redaction workflows; secure storage; secrets management.
- Threat modeling; audit trails; role-based access; rate limiting.
- PWA/mobile-first patterns; offline storage; push notifications.
- Health informatics: HL7/FHIR basics; mapping data fields; SMART-on-FHIR concepts.

**Projects**
- *De-ID Lantern*: redact PHI in text/PDF; export clean notes with audit report.
- *Tea & Symphony — PWA*: journaling + symptom tags; simple trend insights.

**Definition of Done**
- Beta users using weekly; consent flows; export/download; error budgets & monitoring basics.

---

## Phase 5 (Months 19–24): Consulting Engine
**Topics**
- Offers & positioning; pricing; proposals & SOW; lightweight legal & compliance.
- Case studies: problem → solution → impact → demo link.
- Content engine: newsletter cadence; “build in public” posts; short demos.

**Projects**
- Package *Vitals Whisperer* and *Chiron Node* as turnkey installs for clinics.
- Publish 3 case studies and a one‑pager per offer (audit, prototype, automation).

**Definition of Done**
- First paid pilot(s); repeatable sales narrative; testimonial or reference secured.

---

## Phase 6 (Months 25–36): Scale & Specialize
**Topics**
- Cloud IaC (Terraform basics), Docker in prod, observability.
- Fine‑tuning vs. retrieval tradeoffs; eval at scale; safety/compliance reviews.
- Specialty focus (e.g., perioperative pathways; addiction & mental health).

**Projects**
- Production‑grade deployment of the strongest app.
- Lightweight analytics; cohort retention; uptime SLOs.

**Definition of Done**
- Sustainable consulting pipeline; recurring revenue from productized services.

---

## Weekly Cadence (example)
- **Mon**: Learn (2h) + Notes (30m)
- **Tue**: Build feature (2h)
- **Wed**: UX/Design (1h) + Build (1h)
- **Thu**: Data/AI (2h)
- **Fri**: Ship a demo or post (1h)
- **Sat**: Buffer or rest
- **Sun**: Retrospective + plan (30m)

---

## Skill Checklists (abbrev)
- Git: branch/PR/merge, resolve conflicts, rebase safely.
- Python: list/dict comps, exceptions, dataclasses, pytest fixtures.
- Web: REST CRUD, auth, pagination, N+1 detection, indexes.
- SQL: joins, group by, window functions, migrations.
- AI: build a retrieval index, write prompts, measure accuracy, log failures.
- Security: env vars, secret storage, log redaction, basic threat model.
