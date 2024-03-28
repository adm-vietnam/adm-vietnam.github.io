---
layout: home
title: 
description: 
background: /assets/theme/images/chuttersnap-146799-unsplash.jpg
permalink: /
---

<b>Description</b> <br>
<p>
The 2024 ADM is a 6-month program (July - December 2024) to provide undergraduate and master's students with research experience, serving as a stepping stone for students to pursue their Ph.D. at top universities. The program aims to equip students with some of the advanced mathematical knowledge most used in applied research, such as combinatorics, probability, statistics, machine learning, and algorithms. In the next step, the program will direct the most capable students to participate in research projects and obtain meaningful results, suitable for publication in international journals.
</p>

<p>
The program is a great opportunity for participating students to meet, exchange and learn from experts who will provide not only scientific guidance but also orientation for students in finding PhD scholarships at major universities. The program is developed by the VINIF Foundation and the Big Data Research Institute (VinBigdata), with the direct participation of professors Vu Ha Van (Yale/VINIF/VinBigdata), Nguyen Huu Hoi (Ohio State University), Tran Manh Tuan (University of Science and Technology of China), Nguyen Minh Tan (National University of Singapore), Ho Pham Minh Nhat (UT Austin), and some other scientists.  
</p>

<p>
The program consists of two phases: boot camp and distance supervision.  
<ol>
  <li>
Boot camp: The boot camp will takes place (offline) from July 1 to July 31, in Hanoi. It will include lectures (in machine learning, data science, statistical, probability, and combinatorics), discussions on exercises and research topics, and a small conference. Students will receive housing support and a stipend.</b></li>
  <li>
Distance supervision: From August 1 to December 30, mentors will supervise students remotely, focusing on several specific research topics. After December 30, students can continue to work with mentors, depending on the level of development of the project.</li>
</ol>
After the program, each student will:
<ul>
  <li>
    continue receiving advice from their mentor for graduate school applications;</li>
  <li>
    get connected as needed to students with more experience.</li>
</ul>
</p>

<b>Eligibility</b> <br>
This program is open to undergraduate and master's students at Vietnamese universities. Participants must be able to spend the full one month in Hanoi.

<b>Organizers</b> <br>
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

<b>Contact</b> <br>
Email to <a href="mailto:trantuan@ustc.edu.cn">trantuan@ustc.edu.cn</a>.
