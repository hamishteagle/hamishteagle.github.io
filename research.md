---
layout: page
title: Publications
---

{% assign sorted = site.research | sort: 'date' | reverse %}
{% for res in sorted %}
<div class="Publication">
    <h2><a href="{{ res.url }}">{{ res.title }}</a></h2> <embed src="{{ site.url }}/{{ res.pdf }}" type="application/pdf" width="500" height="300" />
  </div>
{% endfor %}