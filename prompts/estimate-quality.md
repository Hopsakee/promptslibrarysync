---
title: "Estimate quality"
tags: ["learning"]
created: "2025-12-20T15:11:26.14904+00:00"
updated: "2026-01-02T12:33:31.783Z"
version: 4
---

I'm about to read the given document.

Task: Judge the likely quality and my likely ROI from reading it, given my interests and current knowledge.

Assume I value:
- Enduring ideas, mental models, and clear conceptual distinctions.
- Strong arguments, synthesis, and well-supported claims.
- References/citations when they are integrated and guide further study.
- Actionable steps are nice-to-have, not required.

Follow these steps:

## Step 0 — Assumed Reader Baseline (no “personal fit”)
Assume the reader is already beyond beginner level in the document’s domain.
- Not “how to start in an hour.”
- Knows fundamentals and common vocabulary.
- Wants depth, conceptual clarity, and well-supported claims.

## Step 1 — Classify the Document (1 label)
Choose exactly one:
A) How-to / tutorial
B) Research / technical report
C) Philosophy / theology / humanities essay (argumentative)
D) History / narrative (story-driven)
E) Reference / survey / literature review
F) Marketing / announcement / demo

Write 1 sentence explaining why you chose it.

## Step 2 — Extract “Instances of Value” (IVs)
Extract ONLY items that would meaningfully change an informed reader’s understanding.
An IV can be ANY of the following:
1) A new mental model / framing that compresses complexity.
2) A precise definition or distinction that resolves confusion (conceptual clarity).
3) A strong argument move: premises → inference → conclusion (including counterarguments).
4) A synthesis that connects domains (bridges ideas that are rarely bridged well).
5) A high-quality “reading map”: references that are curated + contextualized (why each matters).
6) A concrete method/practice/heuristic (optional category, not required).
7) A historically influential or canonical position explained in a way that reveals why it mattered.

IMPORTANT:
- “Mentions” do NOT count. The document must do explanatory work: justify, argue, define, or synthesize.
- You may include 0 IVs if the document is shallow or purely promotional.

## Step 3 — Score EACH IV (0–3) with strict rubric
For every IV, assign points:

Depth (0–3):
0 = mere assertion / slogan
1 = some explanation but thin
2 = clear reasoning or concrete example
3 = deep, layered reasoning OR uniquely clarifying synthesis

Plus 1 bonus point (optional, +0 or +1) IF the IV is unusually enduring (likely valuable in 5–10 years).

IV Score = Depth (0–3) + Endurance Bonus (0–1). Max per IV = 4.

## Step 4 — Score Document Quality (Intrinsic) and ROI (separate)
Compute two separate scores:

A) Intrinsic Quality Score (0–20), sum of:
- Argument/Rigor (0–5): logical structure, handles objections, avoids handwaving (appropriate to doc type)
- Conceptual Clarity (0–5): definitions, distinctions, precision
- Evidence/Support (0–5): citations, examples, credible grounding (appropriate to doc type)
- Coherence/Structure (0–5): organized progression, not meandering

B) ROI Score (0–10), sum of:
- Time-to-value (0–4): How quickly it delivers high-density insight vs setup/fluff.
- Transferability (0–3): How reusable the ideas/models are across contexts (not just this case/topic).
- Marginal insight beyond basics (0–3): How much it goes beyond fundamentals into non-obvious distinctions, arguments, or synthesis (without assuming the reader is a beginner).

## Step 5 — “Reference Handling” Rule (fixes the deferral problem)
References/citations are scored as:
- POSITIVE if they are integrated (author explains why they matter or uses them in an argument).
- NEGATIVE only if the text mostly says “go read X” without adding interpretation or synthesis.

## Step 6 — Final Tier (based on IVs + Intrinsic + ROI)
First compute:
Total Value = (Sum of IV Scores) + Intrinsic Quality (0–20) + ROI (0–10).

Apply this gate:
- If Intrinsic Quality < 8, cap at C (even if it feels exciting).

Tier mapping (use best judgment with these anchors):
- S Tier: Total Value ≥ 40 AND no caps triggered.
- A Tier: 30–39 AND no caps triggered.
- B Tier: 20–29.
- C Tier: 10–19 (or capped to C).
- D Tier: <10.

## Output format (strict)

IMPORTANT: use the following exact JSON structure. Don't add anything else to your response. Strictly follow this JSON structure.

```json
{
  "TIER": "[S/A/B/C/D]",
  "Doc Type": "[A–F]",
  "Intrinsic Quality": "X/20",
  "ROI": "R/10",
  "IV Count": "N",
  "Sum IV Score": "Z",
  "Top Instances of Value (up to 7)": [
    {
      "IV summary": "[IV summary]",
      "Depth": "[0–3]",
      "Endurance": "[+0/+1]",
      "IV Score": "[0–4]"
    }
    // ... up to 7 such objects total
  ],
  "Why this tier": "(2 sentences max)",
  "Verdict": "Read / Skim / Skip (1 line)",
  "What to read instead (optional)": "If skipping, name what kind of source would be higher ROI (e.g., \"a commentary\", \"a survey\", \"the primary paper\")."
}
```