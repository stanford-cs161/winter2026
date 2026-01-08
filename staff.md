---
layout: page
title: Staff / Office Hours
description: A listing of all the course staff members.
nav_order: 9
---
## Office Hours

* Office hour schedule can be found on the [Office Hours Calendar](https://calendar.google.com/calendar/u/0?cid=Y18yNDRhYzZkNzdjNzE2MjA0MDVjMDFmNjhjZmJjMjllOWZmMGI3OTZlMTNmNzM4ZDUyMzc2NDIzNDEzYzg0MDJmQGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20).
* Office hours will be hosted either on Zoom or in person. All in-person OH will be group style, meaning that CAs go over problems in front of groups of students. Remote OH can be group style, where students join breakout rooms for the problem that they are working on, or 1-on-1, where students sign up on the queue on [queue.cs.stanford](https://queue.cs.stanford.edu/queues/33FZ7Pjm646CQAkIFshsyyYfm84). The OH calendar specifies the type of each OH session.

<iframe src="https://calendar.google.com/calendar/embed?src=c_244ac6d77c71620405c01f68cfbc29e9ff0b796e13f738d52376423413c8402f%40group.calendar.google.com&ctz=America%2FLos_Angeles" style="border: 0" width="800" height="600" frameborder="0" scrolling="no"></iframe>

## Staff Contact

* The best way to reach the staff is by making a private post on {% include auxlink name='Ed' %}.
* You may also reach us by email at [cs161-staff-win2526@cs.stanford.edu](mailto:cs161-staff-win2526@cs.stanford.edu) (this mailing list is monitored by the Student Liaison) with any questions or concerns that you do not wish to post on {% include auxlink name='Ed' %}.

{% for role in site.roles %}
{% assign staff = site.staff | where: 'role', role %}
{% assign size = staff | size %}
{% if size == 1 %}
## {{ role }}
{% elsif size > 1 %}
## {{ role }}s
{% endif %}
{% for staffer in staff %}{{ staffer }}{% endfor %}
{% endfor %}