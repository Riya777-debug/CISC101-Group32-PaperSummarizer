# Change Log — 2025-11-30

- Added evidence_mode = "strict" to make sure that only information in the paper is taken to create the summary.
- Added section warning messages: if section < 50 words... to make sure the program has enought information in order to run.

---
## Guardrails Module  
- Do not hallucinate sections.    
- Do not fabricate information.    
- Use text **only from provided sections**.    
- Terminology must match the paper exactly.    
- If flagged as short and lacking detail → inform user section cannot be summarised.    
- If a section was separated during summarisation → inform user.


### Strict Evidence Mode:
- if evidence_mode = "strict" → only include claims, equations and results that apppear in the provided text.
- if not enought information is found → output "This text does not provide enough information about the topic being summarized when it is set to strict evidence mode."

### Section Warming Messages:
- if section < 50 words → "Section very short: summary may be incomplete"
- if section = missing → output "Section skipped: no usable text was provided." 
