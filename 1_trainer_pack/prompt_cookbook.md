# Prompt Cookbook — From Prompt to Publication
Every prompt below is copy-paste ready. Replace `[bracketed]` slots. All work in any mainstream chatbot. Universal suffix — append to any prompt when you want grounding: *"Use only information in this prompt; flag anything you are unsure of."*

## §1 · The R-C-T-F pattern (the master pattern)

| Slot | Content | Example |
|---|---|---|
| **R** — Role | Who the model should be, at what level of expertise | "You are a senior editor at a Q1 journal in computer networks." |
| **C** — Context | What the text is, who reads it, what they know | "The abstract below reports an intrusion-detection study on two public datasets; readers know ML basics, not my subfield." |
| **T** — Task | Exactly ONE job | "Critique it in 5 bullets for specificity, quantified results, and stated limitations. Do NOT rewrite it yet." |
| **F** — Format | Shape of the output | "Format each bullet as: issue → why it matters." |

## §2 · The five patterns (slide 10)

1. **Restructure** — "Reorganize this section as: claim → evidence → limitation. Do not add content."
2. **Critique-me** — "Score this 1–10 for specificity. Quote every overclaim verbatim and give the safer wording."
3. **Style-match** — "Rewrite to match the tone of this sample from my own published writing: [paste ~100 words]. Keep all technical content."
4. **Shorten** — "Cut this to N words. Keep all numbers, citations, and the final claim."
5. **Table-maker** — "Convert this into a markdown table with columns X / Y / Z. If a cell is not in my text, write n/a."

**The iteration loop (slide 9):** ask → *"Score your own answer 1–10 for specificity. List every sentence that is generic and could appear in any paper. Propose a fix for each."* → refine → *"Rewrite fixing all listed issues. Keep every number exactly as in my original."* Stop when the critique turn finds only cosmetic nits.

## §3 · Literature stage

**D2 — Paper summary (slide 13)**
> Summarize this paper for a related-work section. Extract exactly: (1) the gap it claims to fill; (2) the method in two sentences; (3) the headline quantitative result with its number; (4) the stated limitations; (5) two claims I must verify myself. Use only what is in the text below — if something is absent, write NOT STATED. [paste abstract + key sections]

**D3 — Related-work synthesis (slide 14, safe version)**
> Synthesize these three abstracts into one 150-word related-work paragraph ending with the gap my work fills: [your gap]. Cite as (Author, Year) using ONLY the three provided texts. Do not add any source I did not give you.

**D3b — The trap (teaching only, never in production)**
> Now add three more relevant references.
*(Then check what it produced on doi.org — this is how invalid citations are born.)*

**Screening (slide 15)**
> Rank these abstracts by relevance to my question: [question]. For each: relevant / peripheral / irrelevant, plus a one-line reason. [paste 20–30 titles + abstracts]

## §4 · Drafting stage

**D4 — Outline from results (slide 18)**
> Here are my results as bullet points: [paste 5–8 result bullets with numbers]. Propose a results-section outline. For each subsection give: a one-sentence claim, the evidence bullets that support it, and the statistical detail to report. Nested list. Do not invent any result that is not in my bullets. If two bullets conflict, flag it instead of resolving it.

**D5 — Results → abstract (slide 19)**
> Write a structured abstract (Background, Methods, Results, Conclusion) using ONLY these findings: [paste 3–5 findings with exact numbers]. Constraints: max 200 words; the headline number must appear in Results; no claim may go beyond what the findings state; plain verbs; no citations.

**CARS intro sequence (slide 20)**
> Move 1: "Draft 2 opening sentences situating [topic] for readers of [journal], based on these literature notes of mine: [paste]. No citations — I will attach verified ones."
> Move 2: "From my notes, state in 2 sentences what prior work has not addressed: [paste notes]. Mark any statement that goes beyond my notes."
> Move 3: "Polish this contribution statement for clarity and confidence without adding claims: [paste yours]."

**Methods clarity pass (slide 21)**
> Edit this methods text for clarity and consistent terminology. Change no parameter values, no order of operations, no units. [paste]

**Limitations brainstorm (slide 21 — highest-value prompt of the session)**
> List 8 criticisms a skeptical reviewer could raise about this study design. Rank by how damaging they are. Do not soften them. [paste design summary]

**Caption consistency (slide 21)**
> Make all 6 captions follow the same grammar pattern: what is shown, key condition, how to read it. Keep every figure reference number unchanged. [paste captions]

## §5 · Revision stage

**Paragraph→claim map (slide 23)**
> Map each paragraph of this section to the claim it supports, as a two-column list: paragraph → claim. List paragraphs that serve no claim, and claims with no paragraph. [paste section]

**D6 — Reviewer-2 critique loop (slide 24)**
> Act as Reviewer 2 for a top venue in [field]: skeptical, methodologically rigorous, unimpressed. Review the section below. Give: (1) three major methodological objections; (2) two missing comparisons; (3) every overclaim quoted verbatim, each with safer wording. Score the section 1–10. Be harsh. Do not include praise. [paste section]
> Follow-up: "For each objection, propose a revision action: text change, extra analysis, or honest limitation sentence. Never propose fabricating data or citations."

**Tighten (slide 25)**
> Tighten this section. Cut 25% of words. Keep every number, citation, and claim exactly. Replace vague intensifiers with quantities or delete them. Return: replacement list, then final text. [paste]

**D7 — De-template (slide 26)**
> Edit this paragraph to remove generic AI phrasing (e.g., delve, in the realm of, it is worth noting that, plays a crucial role, underscores). Vary sentence length. Prefer concrete verbs and specific quantities. Keep all technical claims and numbers exactly as they are. Return: replacement list, then final text. [paste]

## §6 · Submission stage

**D8a — Reference self-check (slide 31, starts verification)**
> List every reference you have suggested in this conversation. For each, output the DOI if you are confident it exists, or UNVERIFIED. Flag any where you are unsure of the year or journal.

**D8b — Disclosure draft (slide 31)**
> Draft a generative-AI disclosure statement for [publisher] based on: tool [name + version + month]; uses — [tasks and sections]; NOT used for — [data collection / analysis / interpretation / literature search]; all output reviewed and edited by the authors, who take full responsibility. Two sentences, journal-neutral wording.

**Journal fit (slide 34)**
> Here is my title, abstract, and keywords: [paste]. Shortlist 5 candidate journals. For each give: scope fit in one line, typical readership, reputation for review speed, indexing (Scopus/SSCI), and APC if open access. Mark every fact I must verify on the journal website with VERIFY.

**Cover letter (slide 35)**
> Draft a 250-word cover letter to [journal]. Include: why this manuscript fits the journal's scope and recent readership; the one-line contribution; confirmation of originality and no concurrent submission. Tone: confident, plain, zero superlatives.

**Reviewer responses (slide 35)**
> For each reviewer comment below: quote it, classify (accept / clarify / rebut), draft a point-by-point response of max 120 words, and suggest the exact manuscript change with its location. Never propose analyses that were not run. [paste comments]
