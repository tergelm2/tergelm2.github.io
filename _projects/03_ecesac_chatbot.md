---
name: ECESAC Student Chatbot
tools: [Python, TF-IDF, Gradio, Transformers, BeautifulSoup]
image: /assets/projects/ecesac.svg
description: A grounded student-support chatbot with retrieval, source citations, feedback-aware reranking, and sentiment analysis.
---

<div class="case-study-hero">
  <p class="eyebrow">Team project · Information retrieval</p>
  <h1>ECESAC Student Support Chatbot</h1>
  <p>A retrieval-first assistant that answers questions about ECE courses, faculty, advising, registration, and student resources.</p>
  <img src="{{ '/assets/projects/ecesac.svg' | relative_url }}" alt="ECESAC retrieval and feedback pipeline diagram">
</div>

## The problem

Student information exists across course pages, faculty directories, and FAQs. The chatbot brings those sources into one searchable corpus while keeping generated answers grounded in retrieved records.

## How it works

1. A TF-IDF retriever searches course, faculty, and FAQ records.
2. Retrieved context is passed to the language model with strict grounding instructions.
3. The response includes the supporting records and source URLs.
4. Helpfulness votes adjust the likelihood of retrieved records in future searches.
5. Optional department feedback is classified with a three-class sentiment pipeline.

## My contribution

I implemented the integrated chatbot pipeline, including retrieval, contextual prompting, feedback persistence and reranking, faculty scraping, sentiment analysis, and the three-stage Gradio interaction. I also assembled and documented the project’s course, faculty, and FAQ data sources.

<div class="case-study-grid">
  <div class="case-study-stat"><strong>Grounded answers</strong><span>Retrieved records and source links accompany responses</span></div>
  <div class="case-study-stat"><strong>Learning feedback loop</strong><span>Helpfulness signals influence future rankings</span></div>
  <div class="case-study-stat"><strong>Department insight</strong><span>Optional comments are logged with sentiment labels</span></div>
</div>

## Responsible publication

The public copy preserves collaborator attribution. An API credential that appeared in the private repository’s old history was removed from every published commit; runtime secrets are supplied only through environment variables.

<div class="portfolio-actions">
  <a class="portfolio-button portfolio-button-primary" href="https://github.com/tergelm2/ecesac-chatbot" target="_blank" rel="noopener">Source code ↗</a>
</div>
