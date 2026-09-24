---
name: MediScope
tools: [Node.js, MySQL, Cloud SQL, EJS, SQL]
image: /assets/projects/mediscope.svg
description: Four CMS datasets in a relational hospital model, with Cloud SQL-backed search, SQL quality scoring, and trigger-maintained review metrics.
---

<div class="case-study-hero">
  <p class="eyebrow">Team project · Data engineering &amp; database systems</p>
  <h1>MediScope</h1>
  <p>A relational data model and Cloud SQL-backed application that makes U.S. hospital performance data easier to search and interpret.</p>
  <img src="{{ '/assets/projects/mediscope.svg' | relative_url }}" alt="MediScope hospital analytics interface illustration">
</div>

## The problem

The Centers for Medicare & Medicaid Services publishes extensive hospital data, but its measures are distributed across datasets. Our team brought four CMS datasets covering roughly 5,000 U.S. hospitals into a normalized relational model, then built search and quality-scoring workflows on top of it.

## Data engineering and database design

- Structured hospital, quality-measure, user, and review data as related SQL tables with primary and foreign keys.
- Used multi-table queries to aggregate mortality, readmission, complication, and patient-experience measures.
- Served live hospital search from Cloud SQL through parameterized backend queries.
- Used a stored procedure for the Hospital Quality Index and a trigger to maintain review-count and rating aggregates.

## Application capabilities

- Search by hospital name, state, ZIP code, ownership type, and emergency-service availability.
- Compute normalized mortality, readmission, complication, and patient-experience measures in the backend.
- Calculate a weighted Hospital Quality Index through a stored procedure.
- Register, sign in, save hospital selections, and create, edit, or delete reviews.
- Maintain aggregate review counts and ratings through a database trigger.

## My contribution

I connected the application to Cloud SQL and implemented live hospital search across the Node.js backend and EJS frontend. I also built the hospital review experience and backend CRUD operations, then added the SQL trigger that keeps aggregate review statistics synchronized. The broader schema and dataset integration were team work.

<div class="case-study-grid">
  <div class="case-study-stat"><strong>4 CMS datasets</strong><span>Normalized relational model covering roughly 5,000 hospitals</span></div>
  <div class="case-study-stat"><strong>Cloud SQL search</strong><span>Parameterized, multi-field queries connected to the application</span></div>
  <div class="case-study-stat"><strong>SQL automation</strong><span>Quality-index procedure and trigger-maintained review metrics</span></div>
</div>

## Team attribution

MediScope was developed by Team 109—Edward Han, Ayush Chandra, Tergel Myagmarsaikhan, and Miraya Jain—for CS 411 at the University of Illinois Urbana-Champaign. The public repository preserves the original contributor history.

## Project status

The database and review workflow are implemented. The comparison interface, saved-list controls, and interactive HQI weighting were prototype features at the end of the course project. The [team report](https://github.com/tergelm2/mediscope/blob/main/doc/Team%20109%20-%20CS%20411%20Project%20Report.pdf) documents the completed scope and limitations.

<div class="portfolio-actions">
  <a class="portfolio-button portfolio-button-primary" href="https://github.com/tergelm2/mediscope" target="_blank" rel="noopener">Source code ↗</a>
  <a class="portfolio-button" href="https://www.youtube.com/watch?v=KuK6rlonjIg" target="_blank" rel="noopener">Team demo video ↗</a>
</div>
