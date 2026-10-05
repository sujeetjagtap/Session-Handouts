# Reference Verification Checklist
**The rule: no citation enters the manuscript unopened.** A reference suggested by an AI tool is a *candidate*, not a source.

## The 5-step workflow (from slide 30)

**Step 1 — COLLECT.** Extract every reference the AI suggested into one list, in one place. Start with the self-check prompt (cookbook §6, D8a):
> List every reference you have suggested in this conversation. For each, output the DOI if you are confident it exists, or UNVERIFIED. Flag any where you are unsure of the year or journal.

**Step 2 — LOOK UP.** Resolve each item on **doi.org / Crossref / the publisher site** — never via the chatbot that suggested it. Search by title, not by the model's DOI (models also fabricate plausible DOIs).

**Step 3 — OPEN & READ.** Open the actual paper. Abstract at minimum; the relevant section ideally. A real paper that does not support your claim fails this step.

**Step 4 — CONFIRM THE CLAIM.** The source must say what you cite it for. Misattribution ("Author X showed Y" when X showed not-Y) is as damaging as fabrication — and it survives automated checks.

**Step 5 — RECORD.** Only now does it enter your reference manager (Zotero/Mendeley). Add a one-line note of what the source actually supports — future-you writes faster with an audit trail.

## Edge cases that catch people

| Case | What to do |
|---|---|
| **Preprints (arXiv/medRxiv)** | Real, but check whether a peer-reviewed version superseded it — cite the published version when it exists |
| **Same-author, similar-title papers** | LLMs blend two real papers into one hybrid citation; verify the volume/year match the content you need |
| **Translated or non-English sources** | Verify the original title and the translated claim; facts can drift across translation |
| **Retracted papers** | Check Retraction Watch / publisher banner — citing retracted work unknowingly is bad, knowingly is worse |
| **"Review articles said…"** | If you cite a statistic, trace it to the primary source, not the review that mentioned it |
| **Conference paper vs journal extension** | Cite the version you actually read; note the extension when relevant |

## Time budget reality

- Typical draft: 40–80 references. Verification: ~2 minutes each once practised.
- Do it **as you draft**, not the night before submission — a queue of 80 unverified references is why people skip the step.
- If an AI-suggested reference survives all five steps, great — it was a useful search result. But it became trustworthy *because of the workflow, not because of the model*.
