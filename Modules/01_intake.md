# Module 01 — Intake

## Purpose
Collect and validate user inputs.

## Steps
1. Accept inputs:
   - `paper_text`
   - `summary_level` ("short" or "detailed")
   - `flags` (e.g., `evidence_mode = "strict"`)
2. Validate:
   - Ensure `paper_text` is non-empty.
   - Confirm `summary_level` is valid.
   - Check flags are properly formatted.
3. Pass validated inputs to Section Loop.
