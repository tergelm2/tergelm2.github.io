---
name: Internship Finder
tools: [Python, Flask, TF-IDF, PDF, DOCX]
image: /assets/projects/internship-finder.svg
description: A resume-matching application that extracts skills and ranks internship listings with an explainable relevance score.
---

<div class="case-study-hero">
  <p class="eyebrow">Independent project · Applied NLP</p>
  <h1>Internship Finder</h1>
  <p>A resume-aware search tool that ranks internship listings and explains why each result matches.</p>
  <img src="{{ '/assets/projects/internship-finder.svg' | relative_url }}" alt="Internship Finder matching workflow">
</div>

## The problem

Job boards return large result sets but rarely explain which listings best fit a particular resume. Internship Finder extracts resume text, identifies skills and education signals, gathers candidate listings, and ranks them with a transparent scoring model.

## Ranking approach

- TF-IDF cosine similarity between resume and posting text
- Skill keyword overlap
- Education and field-of-study alignment
- Internship and entry-level signals
- A visible score breakdown for every result

## What I learned

The project reinforced the importance of explaining ranking decisions and separating parsing, data collection, and scoring into independently testable modules.
