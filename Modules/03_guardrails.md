# Module 03 — Guardrails

## Purpose
Prevent hallucination and enforce evidence rules.

## Steps
1. If `evidence_mode = "strict"`:
   - Summarize only text explicitly present.
   - No inferred content.
2. Check each section:
   - If missing → add warning.
   - If empty → add warning.
   - If <50 words → add warning.
3. Pass validated summaries + warnings to Rendering.
