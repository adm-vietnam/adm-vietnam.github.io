---
layout: home
title: Application Driven Mathematics REU
description:
background: /assets/theme/images/chuttersnap-146799-unsplash.jpg
permalink: /
---
## Research Experiences for Vietnamese Students
this subsection contains a description of the program.

## Organizers
<div class="row cards mt-4">
{% for member in site.data.Organizers %}
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

        {% if member.researchgate %}
          <li class="list-inline-item">
            <a href="https://researchgate.net/profile/{{ member.researchgate }}"><i class="ai ai-researchgate"></i></a>
          </li>
        {% endif %}
        
        {% if member.googlescholar %}
          <li class="list-inline-item">
            <a href="https://scholar.google.com/citations?user={{ member.googlescholar }}"><i class="ai ai-google-scholar"></i></a>
          </li>
        {% endif %}

        {% if member.twitter %}
          <li class="list-inline-item">
            <a href="https://twitter.com/{{ member.twitter }}"><i class="fab fa-twitter"></i></a>
          </li>
        {% endif %}

        {% if member.mastodon %}
          <li class="list-inline-item">
            <a href="{{ member.mastodon }}"><i class="fab fa-mastodon"></i></a>
          </li>
        {% endif %}

        {% if member.github %}
          <li class="list-inline-item">
            <a href="https://github.com/{{ member.github }}"><i class="fab fa-github"></i></a>
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

## Contacts
- this contains email address(es)
