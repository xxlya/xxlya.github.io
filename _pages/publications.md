---
layout: page
permalink: /publications/
title: publications
description: Selected representative publications, grouped by research theme.
nav: true
nav_order: 2
categories:
  - key: rl
    name: Reinforcement Learning, Reward Modeling &amp; Policy Optimization
  - key: agentic
    name: Agentic Systems, Planning &amp; Optimization
  - key: data
    name: "Data-Centric AI: Valuation, Curation &amp; Synthetic Data"
  - key: eval
    name: Evaluation, Robustness &amp; Verification for Deployment
  - key: optim
    name: Optimization &amp; Distributed (Large-Scale) Learning
  - key: vision
    name: Vision and Multimodal Perception
  - key: biomed
    name: Biomedical &amp; Scientific Discovery
---
<p>For the complete and up-to-date list, please see my <a href="https://scholar.google.com/citations?user=sdENOQ4AAAAJ&amp;hl=en&amp;sortby=pubdate" target="_blank" rel="noopener">Google Scholar</a> profile.</p>

<div class="publications">

{%- for cat in page.categories %}
  <h2 class="category">{{ cat.name }}</h2>
  {% bibliography -f papers -q @*[category={{ cat.key }}]* %}
{% endfor %}

</div>
