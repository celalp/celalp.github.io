---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
projects:
  - title: "Benchmate"
    description: "Benchmate is a data aggreation tool that allows scientists to aggregate data from multiple sources such as public APIs, literature searches, and other data sources. Benchmate includes tools to represent biological data with different data types such as genomes, sequences, protein structures small molecules and more. Benchmate is currently in development and is available on GitHub. Our ultimate goal is to make data collection, analysis and hypothesis generation more accessible and reproducible."
    link: "https://ccmbioinfo.github.io/ccm_benchmate/"
  - title: "Chirpp"
    description: "CHIRPP program is a Canadian program to track trends in child injuries to inform policy and practice. This program has traditionally been done by manual data entry and analysis. We have developped a robust data pipeline with custom trained models to analyze large volumes of data and provide insights to inform policy and practice. Our pipeline is currently in use by the CHIRPP program and can extract large quantities of data in an automated manner from unstructured clinical notes reducing the manual work by >80% and making sure that the data is consistent, accurate and generated in a timely manner."
  - title: "Allergy"
    description: "Nut allergies are a common cause of anaphylaxis in children and adults alike. This project is an ongoing project to analyze, understand and predict the causes and molecular underpinnings of nut allergies. This project is in collaboration with the Eiwegger lab at University of Vienna and other collaborators. We have developed robust statistical models to predict the likelihood of nut allergies. Categorized gut responses to allergen stimuli and more. Our current goals include development of oral immunotherapies, understanding cross and co sensitizations, and development of new biomarkers for nut allergies."
  - title: "Mnemosyne"
    description: "Mnemosyne, the Titan goddess of memory, was the daughter of Uranus and Gaia and mother of the nine muses. Inspired by her role as the source of inspiration and knowledge, this project aims to bring together the different stages of qualitative research into one integrated system. The ultimate goal of this project is to make qualitative research more accessible and reproducible. This project is under heavy development and is currently in alpha. I am planning this project to be open source and available on GitHub."
    link: "https://celalp.github.io/mnemosyne/"
  - title: "Diagnostic RNA-Seq Pipeline"
    description: "Despite advances in genome sequencing, many individuals with rare genetic disorders remain undiagnosed. Transcriptional profiling via RNA-seq can reveal functional impacts of DNA variants and improve diagnosis. We developed a robust pipeline to analyze RNA-seq data and improve diagnosis of rare genetic disorders in a tissue specific manner. This is the first clinically validated diagnostic RNA-seq pipeline in Toronto that is being actively used in SickKids Genome Clinic."
---

These some of my longer term projects that I am currently working on. These projects range from multi year collaborations to smaller scale projects that I am working on in my free time. Not all my publications are reflected in the project list, I am including things that are longer term collaborations or projects that lead to more than just publications.

{% for project in page.projects %}
## {{ project.title }}

{{ project.description }}

{% if project.link %}
[View Project]({{ project.link }})
{% endif %}

---
{% endfor %}
