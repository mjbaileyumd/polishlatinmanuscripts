---
layout: page
title: Manuscript Layouts
permalink: /layouts/
---

## Court Manuscripts

Voluminous manuscript collections of court records from the sixteenth and seventeenth centuries can be found in archives all over Poland. These include city courts, castle courts, land courts, and the national Crown Tribunal. These records share several important characteristics. 

<div class="dw__focus-curtain">xyz</div>

<div>
{% assign texts_list = site.texts | sort:"url" %}
<ul>
{% for node in texts_list %}
  {% if node.title != null and node.url != "/404.html" %}
    <li><a class="sidebar-nav-item{% if page.url == node.url %} active{% endif %}" href="{{ site.baseurl }}{{ node.url }}">{{ node.title }}</a></li>
  {% endif %}
{% endfor %}
</ul>
</div>
