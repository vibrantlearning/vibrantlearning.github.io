---
layout: page
title: Staff
description: A listing of all the course staff members.
---

# Staff

## Instructors

{% assign founders = site.staffers | where: 'role', 'Founder' %}
{% for staffer in founders %}
{{ staffer }}
{% endfor %}

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Teaching Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

## Former Staff
- Alex Hao
- Anant Asthana
- Caleb Tian
- Kyler Mitra
- Nathaniel John
- Sahil Chowdhury
- Siddarth Das
- [Timothy Feng](http://stats.ioinformatics.org/people/7648)
- Viraj Negandhi
