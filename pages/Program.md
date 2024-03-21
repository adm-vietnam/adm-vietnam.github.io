---
layout: default
title: Program
background: /assets/theme/images/chuttersnap-146799-unsplash.jpg
description: Program description.
permalink: /Program/
---

## Projects
- 1
- 2
- 3

## Mentors

<div class="row cards mt-4">
{% for member in site.data.Mentors %}
  <div class="d-flex team-member col-md-6">
    <div class="flex-shrink-0 me-3">
      {% if member.image %}
        <img src="{{ member.image | relative_url }}" alt="{{ member.name }}">
      {% endif %}
    </div>
    <div>
      <h5 id="{{ member.name | strip | url_encode }}">
        {{ member.name }}
        {% if member.affiliation %}
          <small class="text-muted">| {{ member.affiliation }}</small>
        {% endif %}
      </h5>

      {{ member.description | markdownify }}

      <ul class="list-inline">
        {% if member.orcid %}
          <li class="list-inline-item">
            <a href="https://orcid.org/{{ member.orcid }}"><i class="ai ai-orcid"></i></a>
          </li>
        {% endif %}

        {% if member.email %}
          <li class="list-inline-item">
            <a href="mailto:{{ member.email }}"><i class="far fa-envelope"></i></a>
          </li>
        {% endif %}
      </ul>
    </div>
  </div>
{% endfor %}
</div>

## Participants
<div class="row cards mt-4">
  {% for participants in site.data.participants %}
  <p class="col-md-6">{{ participants.info }}</p>
  {% endfor %}
</div>

## Boot camp

- 1
- 2
- 3
