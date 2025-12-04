# Module 02 — Section Loop

## Purpose
Iterate through required sections and apply summary preferences.

## Steps
1. Sections: Title, Problem, Methods, Findings, Limitations, Future Work.
2. For each section:
   - Extract content from `paper_text`.
   - Apply `summary_level`:
     - **Short** → concise paragraph only.
     - **Detailed** → paragraph + bullet list.
3. Store structured results for Guardrails.
