# Weak vs Strong — Pre-captured Before/After Examples
Use these when a live demo lags or the venue has no internet. Each pair shows the prompt, a representative (abbreviated) output, and the commentary to deliver. Outputs below are **representative composites** for training purposes, not real model logs — say so if asked.

---

## Pair 1 · Abstract critique (D1, D5 fallback)

**WEAK PROMPT:** `Improve my abstract.`
**Typical weak output (abbreviated):** "Your abstract is well-structured. Consider making it more concise and highlighting the significance of your findings. You might also strengthen the methodology section and clarify the main contribution…"
**Commentary:** could be pasted under *any* abstract ever written. Zero sentences named. Nothing actionable.

**STRONG PROMPT (R-C-T-F):**
> You are a senior editor at a Q1 journal in computer networks. The abstract below reports an intrusion-detection study on two public datasets. Critique it in 5 bullets for specificity, quantified results, and stated limitations. Do NOT rewrite it yet. Format each bullet as: issue → why it matters.
**Typical strong output (abbreviated):**
- "achieves high accuracy" → no number; every competing paper claims this too.
- "two public datasets" → unnamed; reviewers cannot judge difficulty or comparability.
- No limitation stated → reads as overclaiming; reviewers will supply harsher ones for you.
- "novel deep approach" → novelty is asserted, not located vs prior art.
- No operational constraint (latency/memory) → the deployment story is missing.
**Commentary:** five specific, rankable, fixable findings — from the same model in the same minute.

## Pair 2 · Paper summary (D2 fallback)

**Input:** a real open-access abstract + results (trainer inserts per field).
**Prompt:** the D2 summary prompt with the NOT STATED rule.
**Typical strong output (abbreviated):** Gap: no prior work evaluates X under class imbalance. Method: two-sentence summary. Headline result: F1 0.87 vs 0.79 baseline. Stated limitations: single-domain evaluation. Claims to verify: (a) the 0.79 baseline figure, (b) "first to evaluate under imbalance".
**Commentary:** item (5) is the workflow — the model tells you what to check, then you go check it. Without the NOT STATED rule, absent fields get silently invented.

## Pair 3 · Related-work citations (D3 fallback)

**Prompt B (the trap):** `Now add three more relevant references.`
**Typical trap output (abbreviated):**
- (Smith & Chen, 2023) "Deep learning for imbalanced intrusion detection" — *Computers & Security*.
- (Okafor, 2022) "Class-imbalance aware IDS evaluation" — *IEEE TIFS*.
- (Villanueva & Roy, 2024) "A survey of LLM-based network defense" — *ACM CSUR*.
**Commentary:** author names exist, venues exist, titles sound exactly right — and (typically) at least one of the three does not exist or does not say this. Checking takes 30 seconds on doi.org: paste title → no match, or a match by a different author with a different claim. **This pair is the reason the five-step verification workflow exists.**

## Pair 4 · Prose tightening (D7 fallback)

**BEFORE (43 words):** "It is important to note that the proposed approach, which was developed in order to address the limitations that were identified in the previously described methods, was able to achieve a performance level that was considerably higher than the baseline approaches that were compared against in our experiments."
**AFTER (9 words):** "The proposed approach outperformed all baselines by 12–18% F1."
**What was cut:** throat-clearing opener ("It is important to note that"), nested qualifications, vague intensifier ("considerably"), passive chains ("was able to achieve", "were compared against").
**Commentary:** the replacement list is the control mechanism — you accept or reject each cut; the model never silently drops a number. Generic phrases are replaced by *specifics from your study*, which is both better prose and exactly what human authorship means to a publisher.
