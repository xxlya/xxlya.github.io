---
layout: page
permalink: /publications/
title: publications
description: Selected representative publications, grouped by research theme. For the complete and up-to-date list, please see my <a href="https://scholar.google.com/citations?view_op=list_works&hl=en&user=sdENOQ4AAAAJ&sortby=pubdate">Google Scholar</a>.
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
---
<div class="publications">

{%- for cat in page.categories %}
  <h2 class="category">{{ cat.name }}</h2>
  {% bibliography -f papers -q @*[category={{ cat.key }}]* %}
{% endfor %}

</div>
