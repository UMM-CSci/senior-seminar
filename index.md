---
---

# UMM CSci Senior Seminar

{% assign sorted_seminars = site.seminars | sort:"semester" | reverse | sort:"year" %}
<ul>
{% for seminar in sorted_seminars %}
{% assign seminarurl = seminar.url | replace: 'index.html', '' %}
<li><a href="{{ seminarurl }}">{{ seminar.title }}</a></li>
{% endfor %}
</ul>