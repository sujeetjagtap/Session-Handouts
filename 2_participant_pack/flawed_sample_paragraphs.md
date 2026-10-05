# Flawed Sample Paragraphs (training material)
These samples are **deliberately flawed** for the session's exercises. They are fictional composites written for training — any resemblance to real papers is coincidental. Each section ends with an answer key (facilitator only).

## §1 · Flawed abstract (Exercise 1)

> "In recent years, cybersecurity has become increasingly important, and deep learning has emerged as a powerful tool in this domain. In this paper, we delve into the fascinating realm of intrusion detection and propose a novel deep learning-based approach that achieves significantly better performance than existing methods. Extensive experiments on benchmark datasets demonstrate the effectiveness of our approach, achieving high accuracy. Moreover, our method plays a crucial role in addressing various challenges in the field. It is worth noting that the results underscore the potential of our framework, which can be easily extended to various real-world scenarios and represents a substantial advancement of the state of the art."

**Answer key — what is wrong (10 items):**
1. "In recent years… increasingly important" — empty opening; no reader needs convincing that the field exists. 2. "delve into the fascinating realm" — classic AI-register filler. 3. "novel… powerful… fascinating… crucial… substantial" — assertion inflation, zero evidence. 4. "significantly better" — statistical significance claimed without test or number. 5. "existing methods" — unnamed; no baseline. 6. "benchmark datasets" — unnamed; comparability unknowable. 7. "high accuracy" — the only quantitative slot in the abstract and it holds no number. 8. "plays a crucial role in addressing various challenges" — says nothing, costs twelve words. 9. "easily extended to various real-world scenarios" — scope creep beyond the evidence. 10. No limitation anywhere — flags the whole abstract as overclaimed.

## §2 · Flawed introduction paragraph (Exercises 2 and D6/D7 fallback)

> "The field of network security has undergone a revolutionary transformation with the advent of machine learning. Numerous studies have shown that these techniques are highly effective. However, challenges still remain in this ever-evolving landscape. Various researchers have proposed various approaches to address these challenges, but there is still a significant gap in the literature. Therefore, in this paper, we present a comprehensive solution that addresses all of these issues and opens new horizons for future research."

**Answer key:** every sentence is a placeholder — "numerous studies" (which?), "highly effective" (measured how?), "various… various" (repetition + vagueness), "significant gap" (the gap is never stated — this is a fabricated premise by vagueness), "comprehensive solution… all of these issues" (unfalsifiable claim). CARS diagnosis: Move 1 asserts a revolution without territory; Move 2 claims a gap it cannot name; Move 3 over-occupies. The fix is not style — it is inserting three real, verified citations and one specific, defensible gap.

## §3 · Flawed methods text (extension exercise)

> "The data was preprocessed using standard techniques to ensure quality. Then, we used a deep neural network with some layers to extract features. Hyperparameters were tuned for optimal performance. The model was trained on the training set and evaluated on the test set. All experiments were run multiple times to ensure reliability."

**Answer key:** "standard techniques" (which?), "some layers" (unreproducible), "tuned for optimal performance" (no search space, no seed), no split ratios, no hardware, no run count, no metrics named — a reviewer cannot reproduce or even sanity-check a single step. AI-assist role here is *clarity editing only* (cookbook §4); the technical facts must come from the author's actual protocol.

## §4 · Neutral results bullets (D4/D5 demo input)

Use these field-neutral bullets when a live demo needs input:
- Detection F1: 0.91 vs baseline 0.79 on dataset A (n=42,700 flows)
- On dataset B: F1 0.86 vs baseline 0.81 (gap narrows under class imbalance 100:1)
- False-positive rate at operating point: 1.8% (baseline 3.9%)
- Inference latency: 41 ms/sample on CPU, 6 ms on GPU
- Model size: 0.6B parameters (baseline transformer: 7B)
- Ablation: removing the threat-intel input drops F1 to 0.83 on dataset B
- Caveat: both datasets lack post-2023 attack families
