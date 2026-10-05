# Publisher AI-Policy Cheat Sheet
**Snapshot date: 2026-10-04.** Publisher policies are moving targets (Elsevier and IEEE both revised theirs within the last year). Treat this sheet as a *starting point and a checklist of what to look for* — always confirm against the journal's current author guide before submission.

## The big four, compared

| | **Elsevier** | **Springer Nature** | **IEEE** | **ACM** |
|---|---|---|---|---|
| **AI allowed for** | Improving readability and language of your own writing; not for generating scientific content | Writing assistance with disclosure; scientific content remains the authors' | Language/reading support for your own text; not scientific content creation | Assistance permitted with disclosure of how AI was used |
| **Disclosure required?** | Yes — declaration in the manuscript | Yes — must be documented | Yes — disclosure required | Yes — incl. submission-time statements |
| **Where it goes** | Declaration **before the References** | **Methods** section (or Acknowledgements if no Methods) | **Acknowledgments** section | Per policy: acknowledgment + statements at submission |
| **AI as author?** | Never | Never | Never | Never |
| **Authors remain responsible for** | Everything, including AI-assisted passages | Everything | Everything | Everything |

**The shared pattern:** assistance is permitted → meaningful use must be disclosed → authorship is exclusively human → responsibility never transfers to the tool. If a journal you target deviates from this pattern, read its guide twice.

## How to check a journal's current policy (3 minutes)

1. Open the journal's **"Guide for Authors"** page (not the publisher's general policy page — journals sometimes add specifics).
2. Search the page for: *AI*, *artificial intelligence*, *generative*, *large language model*, *ChatGPT*.
3. Confirm the three things: allowed uses → disclosure wording + placement → authorship rules.
4. Screenshot or PDF the page **on the day you submit** — policies change mid-review, and the terms you submitted under are the ones that should apply.

## Red flags that trigger editorial scrutiny

- Undisclosed AI-sounding prose flagged by editors or reviewers (the risk is trust, not detection per se)
- References that do not resolve — the #1 AI footprint in submissions (see `reference_verification_checklist.md`)
- A disclosure that says only "AI was used in writing" with no specifics — vague disclosures read as concealment
- AI listed anywhere in the author list — desk rejection territory at all four publishers

## Where this snapshot came from

Compiled for the training session "From Prompt to Publication" (2026-10-04) from the publishers' public AI-writing policies current at that date. The sibling project in this series — the multi-agent research prompt suite (v2.1) — maintains the same table with per-venue facts files and a refresh script (`facts/*.yaml`, `scripts/refresh_facts.py`) if your group needs the machine-checkable version.
