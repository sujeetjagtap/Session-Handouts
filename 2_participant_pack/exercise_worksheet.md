# Participant Pack — Hands-on Worksheet
Session: "From Prompt to Publication" · Bring: a laptop with any AI chatbot open, and (ideally) one paragraph from a manuscript you are actually writing.

---

## Exercise 1 (in-session, 5 minutes) — Fix the flawed abstract

**Goal:** run the full prompt pattern on real bad text, and learn to triage the critiques.

1. Open `flawed_sample_paragraphs.md` and copy **§1, the abstract** — or use a paragraph of your own.
2. Write an **R-C-T-F prompt** that asks for *critique first*: one job, output format specified, no rewriting yet. (Cheat sheet: Role = senior editor in your field; Context = what the text is and who reads it; Task = "critique in 5 bullets for specificity, quantified results, and stated limitations"; Format = "issue → why it matters".)
3. Run it. Then run **one critique turn**: "Score your own answer 1–10 for specificity. List every generic sentence. Propose a fix for each." Then **one refine turn**.
4. Answer these two questions in the space below (you will be asked):

> The fix that surprised me: ______________________

> One critique the model got WRONG, and how I knew: ______________________

**Why question 4 matters:** knowing *which* critique is wrong is the human judgment publishers mean by authorship. The model generates candidates; you arbitrate.

## Exercise 2 (this week, 20 minutes) — Pre-live your own review

1. Take one section of your current draft (or flawed samples §2).
2. Run the Reviewer-2 prompt (cookbook §5) with your field filled in.
3. Build a three-column triage table: objection → agree? (Y/N + why) → revision action (text change / extra analysis / honest limitation).
4. Execute the two cheapest text changes. Notice the section is now better than after any "polish" pass.

## Exercise 3 (this week, 10 minutes) — Verification dry-run

1. Ask your assistant for 5 references relevant to your current project (deliberately unconstrained).
2. Run cookbook §6 **D8a** (the self-check prompt) and record: how many DOIs claimed confident? how many flagged UNVERIFIED?
3. Look up **every one of them** on doi.org or Crossref. Tally: exists-and-says-that / exists-but-says-something-else / does not exist.
4. Write down your ratio. That ratio is why the five-step verification workflow is non-negotiable.

## Facilitator debrief guide

- **Timekeeping:** Exercise 1 is a hard 5 minutes; announce at 2 minutes left. Extensions live in Exercises 2–3, which participants take home.
- **Debrief prompts:** "Which fix surprised you?" and "Which critique was wrong — and how did you know?" Collect 2–3 answers aloud; the second one is the teaching moment.
- **Common sticking points:** (a) participants paste the whole flawed file instead of one paragraph — show that context bloat degrades output; (b) participants let the model rewrite in turn one — re-show the "do NOT rewrite yet" line; (c) participants accept the first critique list wholesale — point at exercise 1 question 4.
- **What success looks like:** everyone leaves having seen *specific, wrong-sometimes* critique — useful precisely because they could arbitrate it.
