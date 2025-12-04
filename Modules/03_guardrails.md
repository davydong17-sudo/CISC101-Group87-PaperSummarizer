# Module 03 — Guardrails

## Purpose
Prevent hallucination and enforce evidence rules.

## Variables
- evidence_mode ∈ {"normal", "strict"}

## Steps
1. If `evidence_mode = "strict"`:
   - Only include information explicitly present in `paper_text`.
   - Remove or rewrite any generated content that is not directly supported.
   - No inferred claims or assumptions allowed.
2. For each section:
   - If the extracted section text is missing:
         Add warning: "Warning: This section was missing in the original paper."
   - If the section text is empty:
         Add warning: "Warning: This section was empty in the original paper."
   - If the section text has fewer than 50 words:
         Add warning: "Warning: This section was under 50 words in the original paper."
3. Pass validated summaries + warnings to Rendering.
