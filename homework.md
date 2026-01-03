---
layout: page
title: Homework
description: A listing of all the course homework.
nav_order: 5
---

## General Homework Information
Homeworks 1-3 will be individual submissions, which means that students should type up their own homework. From Homework 4 onwards, paired submissions are permitted, so students can make a single submission for groups of size up to 2.

## Homework

{% assign all_homework = site.components | where: "type", "homework" %}
{% assign visible_homework = all_homework | where_exp: "item", "item.times[0].begin <= site.time" %}

{% for component in visible_homework %}
  {{ component.content }}
{% endfor %}