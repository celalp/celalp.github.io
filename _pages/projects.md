---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
projects:
  - title: "Benchmate"
    tags: ["Open Source", "Python", "Bioinformatics", "API Integration"]
    description: "Benchmate is a data aggregation platform that enables scientists to fetch and integrate biological data from multiple sources including public APIs, literature databases, and molecular structure repositories. It provides specialized data structures for genomes, protein sequences, 3D structures, and small molecules, streamlining data collection and reproducible hypothesis generation."
    link: "https://ccmbioinfo.github.io/ccm_benchmate/"

  - title: "CHIRPP AI & Clinical NLP Pipeline"
    tags: ["Clinical NLP", "PyTorch", "Transformers", "SickKids"]
    description: "The Canadian Hospitals Injury Reporting and Prevention Program (CHIRPP) tracks pediatric injury trends to inform public policy. We engineered a clinical NLP pipeline leveraging fine-tuned transformer models to extract structured diagnostic information from unstructured emergency department clinical notes, reducing manual chart review by over 80% with high precision."

  - title: "Nut Allergy Biomarkers & Predictive Modeling"
    tags: ["Statistical Modeling", "Clinical Immunology", "Multi-Center Study"]
    description: "In collaboration with the Eiwegger Lab (University of Vienna & SickKids), this project develops statistical models to predict food allergy severity and treatment outcomes. We model allergen-induced intestinal contractions and immune responses to discover novel diagnostic biomarkers, analyze co-sensitizations, and optimize oral immunotherapies."

  - title: "Mnemosyne"
    tags: ["Qualitative AI", "Open Source", "Web App"]
    description: "Inspired by the Titan goddess of memory, Mnemosyne is an open-source suite designed to integrate qualitative research workflows. It streamlines data coding, synthesis, and knowledge extraction to make qualitative data analysis transparent, rigorous, and reproducible."
    link: "https://celalp.github.io/mnemosyne/"

  - title: "Diagnostic RNA-Seq Pipeline for Rare Diseases"
    tags: ["Genomics", "RNA-Seq", "Clinical Diagnostics", "Snakemake"]
    description: "Transcriptional profiling via RNA-seq can uncover functional impacts of DNA variants in undiagnosed rare genetic diseases. We built and validated the first clinical-grade diagnostic blood RNA-seq pipeline at SickKids Genome Clinic, automating splice-variant detection, outlier expression calling, and allele-specific expression analysis."
---

<div class="custom-card" style="background: linear-gradient(135deg, #f8fafc 0%, #f1f5f9 100%); margin-bottom: 2rem;">
  <h2 style="margin-top:0; color: var(--color-primary);"><i class="fas fa-project-diagram"></i> Research &amp; Software Projects</h2>
  <p style="margin-bottom:0; color: var(--color-slate-600);">
    These are long-term research initiatives, open-source software packages, and clinical pipeline architectures I have designed and lead. They encompass multi-year scientific collaborations, clinical deployment pipelines at SickKids, and open-source computational tools.
  </p>
</div>

<div class="projects-grid">
{% for project in page.projects %}
  <div class="project-card">
    <div>
      <h3 class="project-title">{{ project.title }}</h3>
      <div class="project-tags">
        {% for tag in project.tags %}
        <span class="badge badge-tech">{{ tag }}</span>
        {% endfor %}
      </div>
      <p class="project-desc">{{ project.description }}</p>
    </div>
    <div>
      {% if project.link %}
      <a href="{{ project.link }}" target="_blank" rel="noopener" class="btn-custom-primary" style="font-size: 0.85rem; padding: 0.45rem 1rem;">
        <i class="fas fa-external-link-alt"></i> View Repository / Project
      </a>
      {% else %}
      <span class="badge badge-venue"><i class="fas fa-hospital-user"></i> Active Clinical / Institutional Project</span>
      {% endif %}
    </div>
  </div>
{% endfor %}
</div>
