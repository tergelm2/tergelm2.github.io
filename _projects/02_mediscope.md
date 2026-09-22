---
name: MediScope
tools: [Node.js, MySQL, Cloud SQL, EJS, SQL]
image: /assets/projects/mediscope.svg
description: A database-focused hospital analytics prototype over CMS data, with search, quality scoring, and a complete review workflow.
---

<div class="case-study-hero">
  <p class="eyebrow">Team project · Database systems</p>
  <h1>MediScope</h1>
  <p>A web application that makes U.S. hospital performance data easier to search, compare, and interpret.</p>
  <img src="{{ '/assets/projects/mediscope.svg' | relative_url }}" alt="MediScope hospital analytics interface illustration">
</div>

## The problem

The Centers for Medicare & Medicaid Services publishes extensive hospital data, but it is distributed across datasets and difficult for patients to interpret. MediScope organizes those records into a relational model and presents them through a focused search and comparison experience.

## Key capabilities

- Search by hospital name, state, ZIP code, ownership type, and emergency-service availability.
- Compute normalized mortality, readmission, complication, and patient-experience measures in the backend.
- Calculate a weighted Hospital Quality Index through a stored procedure.
- Register, sign in, save hospital selections, and create, edit, or delete reviews.
- Maintain aggregate review counts and ratings through a database trigger.

## My contribution

I connected the application to Cloud SQL and implemented live hospital search across the Node.js backend and EJS frontend. I also built the hospital review experience and backend CRUD operations, then added the SQL trigger that keeps aggregate review statistics synchronized.

<div class="case-study-grid">
  <div class="case-study-stat"><strong>Cloud-backed search</strong><span>Parameterized queries over CMS hospital records</span></div>
  <div class="case-study-stat"><strong>Full review workflow</strong><span>Create, read, update, and delete with ownership checks</span></div>
  <div class="case-study-stat"><strong>Database automation</strong><span>Aggregate-review trigger maintained at the data layer</span></div>
</div>

## Team attribution

MediScope was developed by Team 109—Edward Han, Ayush Chandra, Tergel Myagmarsaikhan, and Miraya Jain—for CS 411 at the University of Illinois Urbana-Champaign. The public repository preserves the original contributor history.

## Project status

The database and review workflow are implemented. The comparison interface, saved-list controls, and interactive HQI weighting were prototype features at the end of the course project. The [team report](https://github.com/tergelm2/mediscope/blob/main/doc/Team%20109%20-%20CS%20411%20Project%20Report.pdf) documents the completed scope and limitations.

<div class="portfolio-actions">
  <a class="portfolio-button portfolio-button-primary" href="https://github.com/tergelm2/mediscope" target="_blank" rel="noopener">Source code ↗</a>
  <a class="portfolio-button" href="https://www.youtube.com/watch?v=KuK6rlonjIg" target="_blank" rel="noopener">Team demo video ↗</a>
</div>
