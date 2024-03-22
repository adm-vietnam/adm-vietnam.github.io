---
layout: home
title: Research Experiences for Students
description: Application Driven Mathematics
background: /assets/theme/images/chuttersnap-146799-unsplash.jpg
permalink: /
---
## Description 

<p>
The 2024 ADM-RES aims to provide research experience to undergraduate and master's students, and serve as a
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

<b>Eligibility</b> <br>
This program is open to undergraduate and master's students at Vietnamese universities. Participants must be able to spend the full one month in residence.

<b>Important dates</b> <br>
Application period: April 1 to May 15 <br>
Interview: May 23 to June 7 <br>
Admissions decision: by June 15 <br>
Boot camp: 1-30 July, on-site <br>
Dynamic collaboration: August 1 to December 30

## Organizers
<div class="row cards mt-4">
{% for member in site.data.Organizers %}
  <div class="d-flex team-member col-md-6" style="justify-content: center;">
    <div class="flex-shrink-0 me-3" style="width: 350px;">
      <div style="position: relative;display: flex;justify-content: center;flex-wrap: wrap;flex-direction: column;align-items: center;">
        {% if member.image %}
        <img src="{{ member.image | relative_url }}" alt="{{ member.name }}">
      {% endif %}
        <p id="{{ member.name | strip | url_encode }}" style="text-align: center;">
        <a href="{{ member.homepage }}">{{ member.name }}</a>
        {% if member.affiliation %}
          <br><small class="text-muted">{{ member.affiliation }}</small>
        {% endif %}
      </p>

      {{ member.description | markdownify }}  
      </div>
    </div>
    
  </div>
{% endfor %}
</div>

## Contacts
- If you have any questions, send an email to <a href="mailto:trantuan@ustc.edu.cn">trantuan@ustc.edu.cn</a>.
