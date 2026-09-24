---
layout: page
title: About
permalink: /about/
weight: 3
---

<div class="about-profile">
  <img src="{{ '/assets/images/tergel-headshot.png' | relative_url }}" alt="Portrait of Tergel Myagmarsaikhan">
  <div>
    <p class="eyebrow">About me</p>
    <h1>Tergel Myagmarsaikhan</h1>
    <p>I’m an Information Sciences + Data Science student at the University of Illinois Urbana-Champaign, graduating in December 2026 with a minor in Computer Science. I’m interested in data engineering work that makes complex data reliable and useful.</p>
    <div class="portfolio-actions">
      <a class="portfolio-button portfolio-button-primary" href="{{ '/assets/resume/Tergel_Myagmarsaikhan_Resume_Sept2026.pdf' | relative_url }}" target="_blank" rel="noopener">View resume ↗</a>
      <a class="portfolio-button" href="mailto:{{ site.author.email }}">Email me</a>
      <a class="portfolio-button" href="https://www.linkedin.com/in/{{ site.author.linkedin }}" target="_blank" rel="noopener">LinkedIn ↗</a>
    </div>
  </div>
</div>

## Data engineering experience

As a Data Engineering Intern at Middleby Corporation in summer 2026, I developed and maintained ETL/ELT pipelines across Azure Data Factory, Azure Synapse, and Microsoft Fabric. I worked on moving legacy brand data into a Bronze/Silver/Gold architecture and built a data-validation platform spanning three source systems and more than 35 tables.

In MediScope, a team hospital-analytics project, I connected the application to Cloud SQL, implemented live search and review workflows, and wrote a trigger to maintain aggregate review metrics. I also enjoy applied AI and information-retrieval projects, but data systems are a central part of the work I want to do next.

## Certification

Microsoft Certified: Fabric Data Engineer Associate (DP-700).

## Tools I have worked with

- **Data and cloud:** SQL, Python, Microsoft Fabric, Azure Data Factory, Azure Synapse, Azure Data Lake, Microsoft Purview, MySQL, Cloud SQL, ETL/ELT pipelines
- **Applications and analysis:** JavaScript, Node.js, React, FastAPI, Streamlit, Pandas, NumPy, scikit-learn, and Git

## Experience and projects

<div class="row">
{% include about/timeline.html %}
</div>

## What I value

- **Useful over flashy:** solve a real problem and make the result understandable.
- **Evidence over guesses:** evaluate models, expose assumptions, and measure outcomes.
- **Team ownership:** describe contributions clearly and give collaborators credit.

<div class="portfolio-actions">
  <a class="portfolio-button portfolio-button-primary" href="{{ '/projects/' | relative_url }}">Explore my projects</a>
  <a class="portfolio-button" href="https://github.com/{{ site.author.github }}" target="_blank" rel="noopener">View GitHub</a>
</div>
