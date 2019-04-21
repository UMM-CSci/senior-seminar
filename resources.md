---
title: Resources
order: 3
layout: resource
permalink: /resources/
match_collection: resources
---

# Resources


Resources for Senior Seminar:

<ul>
{% assign sorted_res = site.resources | sort:"order" %}
{% for res in sorted_res %}
<li><a href="{{res.url | relative_url}}">{{res.excerpt | strip_html }}</a></li>
{% endfor %}
</ul>