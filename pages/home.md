---
layout: home
title: Application Driven Mathematics
description: Research Experiences for Students
background: /assets/theme/images/chuttersnap-146799-unsplash.jpg
permalink: /
---
## Description

<p>
The 2024 ADM-REU aims to provide research experience to undergraduate and master's students, and serve as a
stepping stone for participating students to pursue PhD degrees at top universities. Students will spend
some of the time learning the necessary background while doing research. Each student will work in a
team of up to five, under the supervision of renowned experts, on applied or theoretical projects in High
Dimensional Probability, Statistics, Data Science, Machine Learning, or Combinatorics. The team works
towards solving a meaningful research problem, and writing a paper.
</p>  
The format of the program is divided into two parts:
<ol>
  <li>
Boot camp: This part will be held in person, from July 1st to 30th 2024, in Hanoi. For the first
three weeks, students will attend block courses (consisting of lectures and exercises). The block
courses offer an avenue for standardizing the backgrounds of students, and should give a deeper
insight into special fields of research. For the last week of July, students will do research.</li>
  <li>
Dynamic collaboration: we expect that the teams will continue their projects during the
following academic semester.</li>
</ol>
After the program, each student will:
<ul>
  <li>
    continue receiving advice from their mentor for graduate school applications;</li>
  <li>
    get connected as needed to students with more experience.</li>
</ul>

<b>Funding</b> <br>
The program will provide lodging, travel support to and from Hanoi, as well as a stipend for all students.<br>

<b>Eligibility<b> <br>
This program is open to undergraduate and master's students at Vietnamese universities. Participants must be able to spend the full
one month in residence.

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
