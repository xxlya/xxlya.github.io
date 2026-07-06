---
layout: page
permalink: /repositories/
title: repositories
description: A few GitHub profiles and open-source repositories from our research.
nav: true
nav_order: 5
---

## GitHub users

{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-center align-items-stretch">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html user=user %}
  {% endfor %}
</div>
{% endif %}

## GitHub repositories

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-center align-items-stretch">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
