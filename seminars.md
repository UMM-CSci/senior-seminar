---
title: Seminars
order: 2
permalink: /seminars/
layout: seminar
match_collection: seminars
---

<div id="papers">
<input class="search form-control input-block" type="text" placeholder="Search" />
<br>
<table>
<thead>
<tr>
<th>Seminar</th>
<th>Author</th>
<th>Title</th>
<th>Slides</th>
</tr>
</thead>
<tbody class="list">
{% assign grouped_seminars = site.seminars |  group_by:"year"%}
{% for group in grouped_seminars %}
{% assign sorted_seminars = group.items | where_exp:"item", "item.papers" | sort:"semester" | reverse %}
{% for sem in sorted_seminars %}
{% assign pageurl = sem.url | replace: 'index.html', '' | relative_url %}
{% assign sorted_papers = sem.papers | where_exp:"item", "item.break != true" | sort: 'time' %}
{% for paper in sorted_papers %}
<tr>
  <td class="seminar-title"><a href="{{ pageurl }}">{{ sem.title }}</a></td>
  <td class="author">{{ paper.author }}</td>
  <td class="title">{% if paper.pdf %}<a href="{{ pageurl }}{{ paper.pdf }}">{% endif %}{{ paper.title }}{% if paper.pdf %}</a>{% endif %}</td>
  <td>{% if paper.slides %}<a href="{{ pageurl }}{{ paper.slides }}">Slides</a>{% elsif paper.slidesurl %}<a href="{{ paper.slidesurl }}">Slides</a>{% endif %}</td>
</tr>
{% endfor %}
{% endfor %}
{% endfor %}
</tbody>
</table>
</div>

<script type="text/javascript">
	var options = {
		  valueNames: [ 'seminar-title', 'author', 'title' ]
	};

</script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/list.js/1.5.0/list.min.js" integrity="sha256-YqOIp4MygNx9/lcWr5lpcR88Ki/MNMWvJJkH0eK+fHM=" crossorigin="anonymous" onload="var semList = new List('papers', options);"></script>