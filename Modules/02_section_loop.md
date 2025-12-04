# Module 02 — Section Loop

## Purpose
Iterate through required sections and apply summary preferences.

## Variables
- summary_level ∈ {"short", "detailed"}

## Steps
1. Define the ordered sections:
   ["Title", "Problem", "Methods", "Findings", "Limitations", "Future Work"]
2. For each section:
   - Extract content from `paper_text`.

3. Apply conditional logic using `summary_level`:
   - If summary_level == "short":
       • Produce a concise 1–2 sentence paragraph.
   - If summary_level == "detailed":
       • Produce BOTH:
           (a) A full paragraph summary  
           (b) A bullet list containing key points
     
4. Store structured results for Guardrails.
