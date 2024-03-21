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
    <div class="flex-shrink-0 me-3" style="width: 300px;">
      <div style="position: relative;display: flex;justify-content: center;flex-wrap: wrap;flex-direction: column;align-items: center;">
        {% if member.image %}
        <img src="{{ member.image | relative_url }}" alt="{{ member.name }}">
      {% endif %}
        <p id="{{ member.name | strip | url_encode }}">
        <a href="{{ member.homepage }}">{{ member.name }}</a>
        {% if member.affiliation %}
          <small class="text-muted">({{ member.affiliation }})</small>
        {% endif %}
      </p>

      {{ member.description | markdownify }}
      </div>
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
