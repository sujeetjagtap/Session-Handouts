# Demo Cue Script — D1 to D8
Each cue: when, setup, the exact prompt to type, what to point at while it runs, and the fallback if the live demo fails. Keep a blank chat window (and this file) open on the demo machine. Prompts are identical to `prompt_cookbook.md` and to the slides.

**Universal fallback rule:** never stall more than 60 seconds. Announce "the lag gods have spoken", switch to the fallback text, and keep the room's attention on the *difference* the prompt made, not the tool.

---

## D1 · Weak vs Strong Prompt — slide 8, 00:18, 4 min

**Setup:** one chat window; the sample abstract pasted in your notes (any 150-word abstract with one clearly quantified result; a generic one is fine).
**Type 1 (weak):** `Improve my abstract.`
**While it runs:** say nothing; let the room read the vague output ("sounds helpful, changes nothing").
**Type 2 (strong):** the full R-C-T-F prompt (cookbook §1, right column).
**Point at:** the 5 bullets — each names a *specific* sentence-level weakness; ask the room "which bullets could you act on today?" (all of them vs none).
**Fallback:** `weak_vs_strong_examples.md` pair #1 — pre-captured outputs for both prompts.
**Debrief line:** "Same model, same text, same minute. The prompt was the only variable."

## D2 · Paper Summary — slide 13, 00:34, 3 min

**Setup:** an open-access paper related to the room's field; abstract + results section pasted into the prompt.
**Type:** the D2 prompt (cookbook §3).
**Point at:** item (5) — "two claims I must verify myself" — the prompt builds your verification to-do list; and the NOT STATED rule — ask the room what the model would have done with a missing limitation without it (invented one).
**Fallback:** `weak_vs_strong_examples.md` pair #2.
**Bridge:** "Now watch what happens when I ask for references the paper did not give me…" → D3.

## D3 · Related-Work Synthesis + Reality Check — slide 14, 00:37, 5 min

**Setup:** three real abstracts from the room's field; doi.org open in a second tab.
**Type A:** the safe synthesis prompt (cookbook §3, D3).
**Type B (the trap, immediately after):** `Now add three more relevant references.`
**Point at:** the three new citations — confident, plausible, formatted perfectly. Pick one, paste its title into doi.org / Crossref live. Expect: does not exist, or wrong venue/year, or a real paper saying something else.
**Fallback:** the pre-captured failed-citation example in `weak_vs_strong_examples.md` pair #3, plus a narrated doi.org lookup.
**Debrief line:** "This is how tens of thousands of 2025 papers got invalid references (Nature, April 2026). The model wasn't lying — it was completing a pattern."

## D4 · Outline from Results — slide 18, 00:50, 4 min

**Setup:** 6–8 bullet results with numbers (use the sample in `flawed_sample_paragraphs.md` §4 or your own, field-neutral).
**Type:** the D4 prompt (cookbook §4).
**Point at:** claim-evidence pairing per subsection — "this is your argument, drafted"; the conflict-flagging line if it triggers one.
**Fallback:** pre-captured outline in `weak_vs_strong_examples.md` pair #3 commentary.
**Debrief line:** "Notice what it did NOT do: no new numbers, no new findings. The skeleton is yours; it just assembled it."

## D5 · Results → Abstract — slide 19, 00:54, 4 min

**Setup:** same results bullets as D4 (continuity helps the room see the pipeline).
**Type:** the D5 prompt (cookbook §4).
**Point at:** the headline number landing in Results; count the claims that have numbers vs the room's own last abstract; then run the Shorten pattern live if the output exceeds 200 words.
**Fallback:** pre-captured abstract in `weak_vs_strong_examples.md` pair #1 commentary.
**Debrief line:** "'ONLY these findings' is the ethics mechanism — scope creep was blocked by the prompt, not by your vigilance."

## D6 · Reviewer-2 Critique Loop — slide 24, 01:11, 5 min

**Setup:** a genuinely improvable section — your own draft or the flawed intro from `flawed_sample_paragraphs.md` §2.
**Type:** the D6 prompt (cookbook §5), then the follow-up prompt.
**Point at:** one objection you agree with → fix it live in one sentence; one objection that is wrong → triage it like a real review ("reviewers are sometimes wrong; so is the model — your judgment is the same muscle").
**Fallback:** the pre-captured Reviewer-2 report in `weak_vs_strong_examples.md` pair #3.
**Debrief line:** "You just pre-lived December's review in five minutes. Painful now, painless later."

## D7 · De-Templating — slide 26, 01:18, 4 min

**Setup:** a paragraph with 3+ AI-isms (flawed samples §1 or §2 work).
**Type:** the D7 prompt (cookbook §5).
**Point at:** the replacement list — each generic phrase replaced by something *specific from the study*; say plainly: "We edit phrasing because vague prose is weak prose. We never touch numbers or claims. Detectors are not the target; readers are."
**Fallback:** the before/after in slide 25 plus a narrated replacement list.
**Debrief line:** "Specificity is the whole game — and it is exactly what publishers mean by human authorship."

## D8 · Verify References + Draft the Disclosure — slide 31, 01:34, 6 min — THE FINALE

**Setup:** the conversation from D3 still open (it suggested 3 references); doi.org in a tab; your disclosure slot ready (cookbook §6, D8b).
**Type 1:** the D8a self-check prompt. **Point at:** the UNVERIFIED flags — "this is the model being honest for once; trust the flags, not the confident DOIs."
**Then:** paste 2 of the D3 references into doi.org live. Expect at least one failure — let it land in silence for two seconds.
**Type 2:** the D8b disclosure prompt with the session's own uses filled in ("improved phrasing in demos; no role in analysis").
**Point at:** the four disclosure slots appearing in two sentences; show on the journal's author-guidelines page where the statement goes.
**Fallback:** the pre-captured UNVERIFIED table + disclosure text in `integrity_pack/ai_use_disclosure_templates.md`.
**Debrief line:** "Verify before it enters the manuscript; disclose because it did. That is the entire contract."
