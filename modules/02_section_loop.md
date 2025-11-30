# Change Log — 2025-11-24

- Added summary_level variable for identifying whether the summary is short or detailed.
- Added conditional logic to determine what kind of output should proceed if the summary is short or detailed.

---
### Section Loop Module  
```
summary_level = "short" | "detailed"
  For each section selected by the user:  
  - If summary_level = "short" → output **max 3 sentence summary**.
  - If summary_level = "detailed" → output summary + bullet list for each key points
  - If unflagged → output summary of appropriate length.    
  - Cite all summarised information directly from the paper.
```
