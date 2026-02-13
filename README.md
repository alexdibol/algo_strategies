# Algo Strategies — Strategies Under Governance (Synthetic-First)

Governance-first · auditable · reproducible · human-accountable  
Built for **MBA / Master of Finance cohorts** and **professional trading / research practitioners** who need mechanism clarity under constraint.

**Landing page:**  
https://alexdibol.github.io/algo_strategies

---

## What this repository is

This repository is the governed home of **Algo Strategies**: a synthetic-first laboratory suite for implementing and evaluating **canonical strategy archetypes** without relying on any external market data or platform.

Most strategy education over-teaches “signals” and under-teaches **engineering reality**:
costs, turnover, feasibility, regime sensitivity, and the governance required to make any result reviewable.

This pillar is intentionally explicit about its limits:

- it does **not** promise alpha discovery  
- it does **not** claim deployability  
- it does **not** treat backtests as evidence  

It is a mechanism-first research and teaching environment designed to be:

- deterministic under seed  
- synthetic-only (no external data)  
- auditable via mandatory run artifacts  
- constrained by explicit stage gates and “Not verified” outputs

**Core premise:**  
**Capability ↑ ⇒ Risk ↑ ⇒ Controls ↑**

---

## Canonical links

### Landing page
- https://alexdibol.github.io/algo_strategies

### Repository
- https://github.com/alexdibol/algo_strategies

### Notebooks
- Folder: https://github.com/alexdibol/algo_strategies/tree/main/notebooks
- CHAPTER_1: https://github.com/alexdibol/algo_strategies/blob/main/notebooks/CHAPTER_1.ipynb
- CHAPTER_2: https://github.com/alexdibol/algo_strategies/blob/main/notebooks/CHAPTER_2.ipynb
- CHAPTER_3: https://github.com/alexdibol/algo_strategies/blob/main/notebooks/CHAPTER_3.ipynb
- CHAPTER_4: https://github.com/alexdibol/algo_strategies/blob/main/notebooks/CHAPTER_4.ipynb
- CHAPTER_5: https://github.com/alexdibol/algo_strategies/blob/main/notebooks/CHAPTER_5.ipynb
- CHAPTER_6: https://github.com/alexdibol/algo_strategies/blob/main/notebooks/CHAPTER_6.ipynb
- CHAPTER_7: https://github.com/alexdibol/algo_strategies/blob/main/notebooks/CHAPTER_7.ipynb
- CHAPTER_8: https://github.com/alexdibol/algo_strategies/blob/main/notebooks/CHAPTER_8.ipynb
- CHAPTER_9: https://github.com/alexdibol/algo_strategies/blob/main/notebooks/CHAPTER_9.ipynb
- CHAPTER_10: https://github.com/alexdibol/algo_strategies/blob/main/notebooks/CHAPTER_10.ipynb

### Book
- Folder: https://github.com/alexdibol/algo_strategies/tree/main/book
- PDF: https://github.com/alexdibol/algo_strategies/blob/main/book/BOOK%20STRATEGY%20FOR%20TRADERS.pdf
- Notes: https://github.com/alexdibol/algo_strategies/blob/main/book/readme.md

---

## Strategy index (10 governed notebooks)

Each chapter is a strategy archetype implemented as **one Colab notebook** with the full governed pipeline.

1) **CAPM Alpha Ranking**  
2) **Fundamental Factor Long–Short**  
3) **Style Rotation**  
4) **Momentum + Market Risk Gate**  
5) **Turn-of-the-Month Seasonality**  
6) **Short-Term Reversal**  
7) **Momentum–Reversal Hybrid**  
8) **Pairs Trading**  
9) **Dynamic Breakout**  
10) **Futures Trend + Carry**

---

## What every notebook enforces (non-negotiable)

This repository uses a strict “laboratory contract.” Every notebook:

- is **Python only**
- uses **synthetic data only**
- is **deterministic under seed**
- uses **basic Python types** (lists/dicts) and standard libraries
- **forbids pandas** (no pandas whatsoever)
- implements the full pipeline:

  synthetic market construction → signal isolation → portfolio rules → costs/slippage → stress tests → stage gates → artifact logging → deliverables

- runs end-to-end and produces a governed artifact bundle each run, including:

  - `run_manifest.json`
  - `prompts_log.jsonl`
  - `risk_log.json`
  - `deliverables/` outputs per run (metrics, diagnostics, equity curve, positions, stress results, and gate decision)

- marks all outputs:

  - `verification_status="Not verified"`
  - with **facts_provided vs assumptions vs open_items** separated

This is not “extra process.”  
This is what makes strategy work defensible.

---

## How to use this repository

Recommended learning posture:

1) Read the book first (mechanism framing and governance posture).  
2) Run a notebook as-is (no tuning).  
3) Inspect artifacts and diagnostics.  
4) Stress the system structurally (not by optimizing).  
5) Document failures and stage-gate outcomes.  
6) Only then modify a single mechanism at a time.

**Operating rule:** If the notebook “works” only when you ignore costs, liquidity, or constraints, then it does not work.

---

## Shared governance spine (applies across this repo)

- **Generation ≠ verification**  
  Model output is always **Not verified** until qualified humans validate it.

- **Facts vs assumptions discipline**  
  Facts provided, assumptions made, and open questions are explicitly separated.

- **Scope and boundary control**  
  Clear task definitions, stop-if rules, and refusal posture where applicable.

- **Auditability by design**  
  Artifacts enable reconstruction, supervision, and review.

- **Human accountability**  
  Responsibility never leaves the human professional.

- **Synthetic-first honesty**  
  These are controlled laboratories to study mechanisms, not claims about real markets.

---

## Who this is for

Designed for:

- MBA and Master of Finance students  
- systematic traders and researchers  
- risk, compliance, and model governance teams  
- instructors teaching algorithmic strategy responsibly  
- practitioners who want mechanism clarity before performance narratives  

This is not a “get-rich” repository.  
The objective is **mechanism literacy** and **governed experimentation**.

---

## Use of generative AI tools (transparency statement)

Generative AI tools may have been used to assist drafting, editing, formatting, or code scaffolding.

However:

- conceptual design  
- pedagogical structure  
- governance logic and control definitions  
- integration decisions  
- final editorial judgment and acceptance  

were **human-led, human-supervised, and human-approved** at all times.

The author assumes **full responsibility** for the content, structure, interpretation, and conclusions presented in this work.

---

## IMPORTANT DISCLAIMERS (read before use)

### Educational / Non-Reliance
All materials are provided **for educational and research purposes only**.  
Nothing in this repository constitutes:

- investment advice  
- trading advice  
- legal advice  
- tax advice  
- accounting or audit advice  
- compliance determinations  
- operational recommendations  

Qualified human professionals must review, verify, and approve any real-world use.

### Not verified
Unless explicitly stated otherwise in a particular artifact, treat all outputs, claims, calculations, citations, and conclusions as **Not verified**.

### Confidentiality and data hygiene
Do not paste confidential, proprietary, regulated, or personally identifying information into external systems.  
Use anonymization/redaction and **minimum-necessary** inputs by default.  
You are responsible for compliance with privacy, confidentiality, recordkeeping, and information security obligations.

### No fabricated sources or claims
Zero tolerance for invented citations, performance claims, fees, terms, or consequences.  
When evidence is missing, the correct output is a **verification task list**, not persuasive narrative.

---

## License (MIT)

This project is released under the **MIT License**.

**Copyright (c) 2026 Alejandro Reynoso**

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

## Contact

Alejandro Reynoso  
Email: areynoso@yahoo.com  
GitHub: https://github.com/alexdibol
