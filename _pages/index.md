---
layout: single
title: "Alper Celik, Ph.D."
permalink: /
excerpt: "Senior Bioinformatician & Data Scientist specializing in machine learning, high-performance computing, clinical NLP, and multi-omics data integration."
author_profile: true
---

<div class="hero-card">
  <span class="hero-badge"><i class="fas fa-microscope"></i> Data Science &amp; Bioinformatics</span>
  <h1 class="hero-title">Advancing Medicine &amp; Biology with Data Science</h1>
  <p class="hero-subtitle">
    I am a Senior Bioinformatician at SickKids with a Ph.D. focused on developing predictive machine learning algorithms, scalable multi-omics pipelines, and clinical NLP tools that translate complex biological datasets into actionable discoveries.
  </p>
  <div class="hero-actions">
    <a href="/papers/" class="btn-custom-primary"><i class="fas fa-file-alt"></i> View Publications</a>
    <a href="/projects/" class="btn-custom-secondary"><i class="fas fa-code-branch"></i> Explore Projects</a>
    <a href="/about/" class="btn-custom-secondary"><i class="fas fa-user-circle"></i> About &amp; Resume</a>
  </div>
</div>

<div class="stats-grid">
  <div class="stat-card">
    <div class="stat-value">15+</div>
    <div class="stat-label">Peer-Reviewed Papers</div>
  </div>
  <div class="stat-card">
    <div class="stat-value">99%+</div>
    <div class="stat-label">Clinical NLP Accuracy</div>
  </div>
  <div class="stat-card">
    <div class="stat-value">&gt;80%</div>
    <div class="stat-label">Manual Review Reduction</div>
  </div>
  <div class="stat-card">
    <div class="stat-value">100+</div>
    <div class="stat-label">Omics Datasets Analyzed</div>
  </div>
</div>

## <i class="fas fa-newspaper" style="color: var(--color-primary);"></i> Featured Research

{% assign sorted_papers = site.pages | where: "permalink", "/papers/" | first %}
{% for paper in sorted_papers.papers limit:3 %}
<div class="publication-item">
  <div class="pub-title">{{ paper.title }}</div>
  <div class="pub-meta">
    <span class="badge badge-venue"><i class="fas fa-journal-whills"></i> {{ paper.venue }}</span>
    <span><i class="far fa-calendar-alt"></i> {{ paper.date }}</span>
  </div>
  <div class="pub-authors">
    <strong>Authors:</strong> {{ paper.authors }}
  </div>
  {% if paper.synopsis %}
  <div class="pub-synopsis">
    <strong>Key Insight:</strong> {{ paper.synopsis }}
  </div>
  {% endif %}
  {% if paper.link and paper.link != '*Coming Soon*' %}
  <a href="{{ paper.link }}" target="_blank" rel="noopener" class="project-link">
    Read Publication <i class="fas fa-external-link-alt"></i>
  </a>
  {% else %}
  <span class="badge badge-tech"><i class="fas fa-clock"></i> In Press / Coming Soon</span>
  {% endif %}
</div>
{% endfor %}

<div style="text-align: right; margin-bottom: 2.5rem;">
  <a href="/papers/" class="project-link" style="font-size: 1rem; font-weight: 700;">View All Publications &rarr;</a>
</div>

---

## <i class="fas fa-cubes" style="color: var(--color-primary);"></i> Featured Projects

<div class="projects-grid">
{% assign sorted_projects = site.pages | where: "permalink", "/projects/" | first %}
{% for project in sorted_projects.projects limit:4 %}
  <div class="project-card">
    <div>
      <h3 class="project-title">{{ project.title }}</h3>
      <p class="project-desc">{{ project.description | truncatewords: 32 }}</p>
    </div>
    <div>
      {% if project.link %}
      <a href="{{ project.link }}" target="_blank" rel="noopener" class="project-link">
        Explore Project <i class="fas fa-arrow-right"></i>
      </a>
      {% else %}
      <span class="project-link" style="color: var(--color-slate-500) !important;">
        Active Collaboration
      </span>
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>

<div style="text-align: right; margin-top: 1rem;">
  <a href="/projects/" class="project-link" style="font-size: 1rem; font-weight: 700;">Browse All Projects &rarr;</a>
</div>