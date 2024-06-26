---
layout: home
title: 
description: 
background: /assets/theme/images/chuttersnap-146799-unsplash.jpg
permalink: /4.html
---

<b>Description</b> <br>
<p>
The 2024 ADM is a 6-month program (July - December 2024) designed to offer research experience to undergraduate, master's, and recent students, serving as a foundational platform for students to pursue their PhDs at top universities. The program aims to equip students with some of the advanced mathematical knowledge most used in applied research, such as combinatorics, probability, statistics, machine learning, and algorithms. In the next step, the program will direct the most capable students to participate in research projects and obtain meaningful results, suitable for publication in international journals.
</p>

<p>
The program is a great opportunity for participating students to meet, exchange and learn from experts who will provide not only scientific guidance but also orientation for students in finding PhD scholarships at major universities. The program is developed by the VINIF Foundation and the Big Data Research Institute (VinBigdata), with the direct participation of professors Vũ Hà Văn (Yale/VINIF/VinBigdata), Nguyễn Hữu Hội (Ohio State University), Trần Mạnh Tuấn (University of Science and Technology of China), Nguyễn Minh Tân (National University of Singapore), Hồ Phạm Minh Nhật (UT Austin), and some other scientists.  
</p>

<p>
The program consists of two phases: summer school and distance mentoring.  
<ol>
  <li>
Summer school: This will takes place from July 1 to July 31 (offline), in Hanoi. It will include lectures (in machine learning, data science, statistical, probability, and combinatorics), discussions on exercises and research topics, and a small conference. Each student will receive 10 million VND.</li>
  <li>
Distance mentoring: From August 1 to December 30, mentors will supervise students remotely, focusing on several specific research topics. After December 30, students can continue to work with mentors, depending on the level of development of the project.</li>
</ol>
After the program, each student will:
<ul>
  <li>
    continue receiving advice from their mentor for graduate school applications;</li>
  <li>
    get connected as needed to students with more experience.</li>
</ul>
</p>

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
