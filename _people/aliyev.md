---
layout: single
permalink: /people/aliyev/
author_profile: true
---

{% assign prof = site.data.professors | where: "id", "aliyev" | first %}

# {{ prof.name }}

## 🧑‍🏫 Position
{{ prof.position }}

## 🔬 Field
{{ prof.field }}

## 📖 About
Researcher in solar radio bursts and CME analysis.

## 📄 Publications
<ul>
{% for pub in prof.publications %}
  <li><a href="{{ pub.link }}">{{ pub.title }}</a></li>
{% endfor %}
</ul>

## 📧 Contact
{{ prof.email }}
