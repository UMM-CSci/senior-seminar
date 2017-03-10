---
title: Home
order: 1
layout: base
---

<div class="jumbotron">
<div class="container">
  <h1>Senior Seminar</h1>
  <p>Computer Science at the University of Minnesota Morris</p>
</div>
</div>

<div class="container about-that">
<div class="columns">
  <div class="one-half column">
    <h2>{{ site.seminars | size }} Past Seminars</h2>
    <p>View papers and slides from past senior seminars</p>
    <a href="{{ "/seminars/" | relative_url }}" class="btn btn-outline" role="button">View Seminars</a>
  </div>
  <div class="one-half column">
    <h2>Resources</h2>
    <p>Resources for students</p>
    <a href="{{ "/resources/" | relative_url }}" class="btn btn-outline" role="button">View Resources</a>
  </div>
</div>
</div>

<span class="octicon octicon-tools"></span>